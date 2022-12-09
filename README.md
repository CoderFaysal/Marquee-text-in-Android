# Marquee text in Android


### The XML file with the textview:

```
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="fill_parent"
    android:layout_height="fill_parent"
    >
    
    
    <TextView
        android:id="@+id/text"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentRight="true"
        android:singleLine="true"
        android:ellipsize="marquee"
        android:fadingEdge="horizontal"
        android:marqueeRepeatLimit="marquee_forever"
        android:scrollHorizontally="true"
        android:textColor="#ff4500"
        android:text="Simple application that shows how to use marquee, with a long text" 
        />
        
        
        
</RelativeLayout>
```


### The JAVA file with the textview:

```
public class TextViewMarquee extends Activity {

   TextView text;
    
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.main);
        
        text = findViewById(R.id.text);  
        
        text.setSelected(true);  // Set focus to the textview
        
        
    }
}
```


_© All Right Reserved by Innovative Programmer ❤️_


