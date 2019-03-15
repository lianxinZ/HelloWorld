#实验一：
##1.创建hello world程序
###关键代码：
~~~
 <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
~~~
###结果截图：
<img src="https://github.com/lianxinZ/project1/blob/master/images/project1-1.jpg" width="250" height="450"/>

##2.验证Activity的生命周期
###关键代码：
~~~
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.d("MainActivityLife","调用onCreate");
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.d("MainActivityLife","调用onStart");
    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.d("MainActivityLife","调用onResume");
    }
    @Override
    protected void onPause(){
        super.onPause();
        Log.d("MainActivityLife","调用onPause");
    }
    @Override
    protected void onStop(){
        super.onStop();
        Log.d("MainActivityLife","调用onStop");

    }
    protected void onDestroy(){
        super.onDestroy();
        Log.d("MainActivityLife","调用onDestroy");

    }
    protected void onRestart(){
        super.onRestart();
        Log.d("MainActivityLife","调用onRestart");

    }

}
~~~
###结果截图：
<img src="https://github.com/lianxinZ/project1/blob/master/images/project1-2.png" width="800" height="250"/>
