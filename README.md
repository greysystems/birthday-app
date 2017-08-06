# birthday-app
android birthday card application.

-----> XML  CODE

<?xml version="1.0" encoding="utf-8"?>

<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/content_activityutama"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    app:layout_behavior="@string/appbar_scrolling_view_behavior"
    tools:context="helloworld.helloworld.Activityutama"
    tools:showIn="@layout/activity_utama"
    android:background="@drawable/cake"
        >

        <TextView
            android:id="@+id/textView"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="happy birthday !!"
            android:textAllCaps="true"
            android:textSize="40sp"
            android:textColor="#263238"
            android:fontFamily="cursive"
            />

        <TextView
            android:id="@+id/textView1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="28 july"
            android:textAllCaps="true"
            android:textColor="@android:color/holo_red_light"
            android:textSize="40sp"
            android:layout_alignParentBottom="true"
            android:layout_centerHorizontal="true"
            android:fontFamily="serif"
            />

</RelativeLayout>


-----> main activity java code

package helloworld.helloworld;
import android.os.Bundle;
import android.support.v7.app.AppCompatActivity;
import android.widget.TextView;
public class Activityutama extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        setContentView(R.layout.activity_utama);
        final TextView helloTextView = (TextView) findViewById(R.id.textView);

        setContentView(R.layout.activity_utama);
        final TextView helloTextView1 = (TextView) findViewById(R.id.textView1);

    }
}


------> screenshot

![screenshot_2017-08-06-05-51-54](https://user-images.githubusercontent.com/17800064/29006081-7b6a5938-7b06-11e7-9762-514b612183ac.png)


-------> HOW TO DEVELOP

Firstly, in XML code everything can be written in RELATIVE LAYOUT which provides us the facility to positioning of texts and images relative to eachother
   
                          1. picture
   
Picture can be displayed by using " android:background="@drawable/cake" ". Firstly, download a cake picture and put that image in drawable folder of that particular application and then by using this statement the image will be displayed.Also the positioning of the image in the screen can be altered or changed by using " android:scaleType="centre or centrecrop" " and many more positions.The positioning up of image can be done by using "wrap_content" (which will wrap the specified space) or "match_parent" (which will cover the whole screen) when you use "IMAGE VIEW" for displaying image.  

                         2. TEXT's
                         
The message or text will be displayed by using " android:text="text" " and textcolor , text background , textsize , textfont can  be changed and positioning of text in the screen too .                        


