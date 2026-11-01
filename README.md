# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: Vikaskumar M
Registeration Number : 212224220122
*/
```
## MainActivity.java
``` python
package com.example.exp_01;

import android.os.Bundle;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;


public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"onCreate Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"onRestart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"onStop Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"onDestroy Called",Toast.LENGTH_LONG);
        toast.show();
    }
}
```
## activity_main.xml

```python
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <ImageView
        android:id="@+id/imageView4"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:scaleType="centerCrop"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="1.0"
        app:srcCompat="@drawable/pd1"
        tools:srcCompat="@drawable/pd1" />

    <TextView
        android:id="@+id/text1"
        android:layout_width="384dp"
        android:layout_height="61dp"
        android:fontFamily="cursive"
        android:text="This is my First Application"
        android:textAlignment="center"
        android:textAllCaps="false"
        android:textColor="#FDFDFD"
        android:textColorLink="#FFFFFF"
        android:textSize="34sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/top2"
        app:layout_constraintVertical_bias="0.471" />

    <TextView
        android:id="@+id/top2"
        android:layout_width="406dp"
        android:layout_height="88dp"
        android:layout_marginTop="176dp"
        android:fontFamily="sans-serif-smallcaps"
        android:text="Welcome to Android Studio"
        android:textAlignment="center"
        android:textColor="#212C49"
        android:textSize="34sp"
        android:textStyle="bold"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="361dp"
        android:layout_height="64dp"
        android:fontFamily="sans-serif-smallcaps"
        android:text="Life Cycle of Android Application Development"
        android:textAlignment="center"
        android:textColor="#000000"
        android:textSize="28sp"
        app:layout_constraintBottom_toTopOf="@+id/text1"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.503"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/top2"
        app:layout_constraintVertical_bias="0.56" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="234dp"
        android:layout_height="48dp"
        android:layout_marginEnd="32dp"
        android:layout_marginBottom="80dp"
        android:fontFamily="cursive"
        android:text="Vikaskumar M"
        android:textColor="#000000"
        android:textSize="30sp"
        android:textStyle="bold|italic"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```


## OUTPUT
<img width="1171" height="689" alt="Screenshot 2026-11-01 181131" src="https://github.com/user-attachments/assets/ac7202b1-a1c0-4074-a31a-0238afeb595b" />

<img width="1147" height="690" alt="Screenshot 2026-11-01 181218" src="https://github.com/user-attachments/assets/de8c99a8-c66a-402a-88e4-d9a9530dd44d" />

<img width="1144" height="683" alt="Screenshot 2026-11-01 181238" src="https://github.com/user-attachments/assets/44cf10ef-675a-4c81-9807-fc38ca51d33a" />

<img width="1148" height="682" alt="Screenshot 2026-11-01 181245" src="https://github.com/user-attachments/assets/4aded380-115d-4c0f-a534-3e897220882a" />

<img width="1148" height="687" alt="Screenshot 2026-11-01 181349" src="https://github.com/user-attachments/assets/c1783e25-0cdd-4dfe-a64f-110eb8a73ccf" />

<img width="1229" height="657" alt="image" src="https://github.com/user-attachments/assets/024a3ce2-4fe6-481c-bb41-a0fefd6f2336" />

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
