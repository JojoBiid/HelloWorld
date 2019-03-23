# HelloWorld & Activity 生命周期
# ![HelloWorld截图](https://github.com/JojoBiid/HelloWorld/blob/master/pic/HelloWorld.jpg)
# ![生命周期截图](https://github.com/JojoBiid/HelloWorld/blob/master/pic/Activity.jpg)
# 关键代码↓
```
package com.example.jojo.helloworld;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;


public class MainActivity extends AppCompatActivity {
    final String TAG = "--MainActivity--";
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        //输出日志
        Log.d(TAG, "-----onCreate-----");
        //
    }
    @Override
    public void onStart() {
        super.onStart();
        //
        Log.d(TAG, "------onStart-------");
    }

    @Override
    public void onRestart() {
        super.onRestart();
        //
        Log.d(TAG, "------ onRestart-------");
    }

    @Override
    public void onResume() {
        super.onResume();
        //
        Log.d(TAG, "------onResume-------");
    }

    @Override
    public void onPause() {
        super.onPause();
        //
        Log.d(TAG, "------onPause-------");
    }

    @Override
    public void onStop() {
        super.onStop();
        //
        Log.d(TAG, "------onStop-------");
    }

    @Override
    public void onDestroy() {
        super.onDestroy();
        //
        Log.d(TAG, "------onDestroy-------");
    }
}
```
