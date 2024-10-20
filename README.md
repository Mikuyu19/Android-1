<!doctype html>
<html>
<head>
<meta charset='UTF-8'><meta name='viewport' content='width=device-width initial-scale=1'>
<title>课后作业1</title>
</head>
<body><h1 id='android课后作业1'>Android课后作业1</h1>
<p>完成课本36页：制作一个登录与注册界面</p>
<p>源文件代码已上传至GitHub</p>
<p>地址：</p>
<h2 id='完成示例图'>完成示例图：</h2>
<p><img src="https://s2.loli.net/2024/10/20/PhQ9R8cf2ItAsUX.jpg" alt="test.jpg" style="zoom:33%;" /></p>
<p>制作相关代码</p>
<h2 id='主界面layoutmain'>主界面Layout_main</h2>
<p>&nbsp;</p>
<pre><code class='language-xml' lang='xml'>&lt;?xml version=&quot;1.0&quot; encoding=&quot;utf-8&quot;?&gt;
&lt;LinearLayout xmlns:android=&quot;http://schemas.android.com/apk/res/android&quot;
    xmlns:app=&quot;http://schemas.android.com/apk/res-auto&quot;
    xmlns:tools=&quot;http://schemas.android.com/tools&quot;
    android:layout_width=&quot;match_parent&quot;
    android:layout_height=&quot;match_parent&quot;
    android:orientation=&quot;vertical&quot;
    android:padding=&quot;10dp&quot;
    android:background=&quot;@drawable/c&quot;
    tools:context=&quot;.MainActivity&quot;&gt;

    &lt;ImageView
        android:id=&quot;@+id/android_icon&quot;
        android:layout_width=&quot;96dp&quot;
        android:layout_height=&quot;96dp&quot;
        android:layout_gravity=&quot;center&quot;
        android:layout_marginTop=&quot;150dp&quot;
        android:src=&quot;@drawable/android_icon&quot; /&gt;

    &lt;EditText
        android:id=&quot;@+id/et_username&quot;
        android:layout_width=&quot;match_parent&quot;
        android:layout_height=&quot;50dp&quot;
        android:layout_marginTop=&quot;50dp&quot;
        android:background=&quot;@drawable/bg_username&quot;
        android:drawableStart=&quot;@drawable/ic_username&quot;
        android:drawablePadding=&quot;8dp&quot;
        android:hint=&quot;用户名&quot;
        android:textColor=&quot;@color/white&quot;
        android:inputType=&quot;text&quot;
        android:padding=&quot;10dp&quot;
        android:textSize=&quot;16sp&quot; /&gt;

    &lt;EditText
        android:id=&quot;@+id/et_password&quot;
        android:layout_width=&quot;match_parent&quot;
        android:layout_height=&quot;50dp&quot;
        android:drawableStart=&quot;@drawable/ic_password&quot;
        android:drawablePadding=&quot;8dp&quot;
        android:layout_marginTop=&quot;5dp&quot;
        android:background=&quot;@drawable/bg_username&quot;
        android:hint=&quot;密码&quot;
        android:textColor=&quot;@color/white&quot;
        android:inputType=&quot;textPassword&quot;
        android:padding=&quot;10dp&quot;
        android:textSize=&quot;16sp&quot;
        /&gt;
    &lt;LinearLayout
        android:layout_width=&quot;match_parent&quot;
        android:layout_height=&quot;wrap_content&quot;
        android:layout_marginTop=&quot;20dp&quot;
        android:orientation=&quot;horizontal&quot;&gt;

        &lt;Button
            android:id=&quot;@+id/btn_login&quot;
            android:layout_width=&quot;0dp&quot;
            android:layout_height=&quot;50dp&quot;
            android:layout_gravity=&quot;center&quot;
            android:gravity=&quot;center&quot;
            android:layout_weight=&quot;1&quot;
            android:background=&quot;@drawable/btn_left&quot;
            android:text=&quot;登录&quot;
            android:textColor=&quot;@color/white&quot;
            android:textSize=&quot;16sp&quot;/&gt;

        &lt;Button
            android:id=&quot;@+id/btn_register&quot;
            android:layout_width=&quot;0dp&quot;
            android:layout_height=&quot;50dp&quot;
            android:layout_gravity=&quot;center&quot;
            android:layout_marginLeft=&quot;5dp&quot;
            android:layout_weight=&quot;1&quot;
            android:background=&quot;@drawable/btn_right&quot;
            android:gravity=&quot;center&quot;
            android:text=&quot;注册&quot;
            android:textColor=&quot;@color/white&quot;
            android:textSize=&quot;16sp&quot; /&gt;

    &lt;/LinearLayout&gt;

&lt;/LinearLayout&gt;
</code></pre>
<p>&nbsp;</p>
<h2 id='mainactivityjava'> MainActivity.java</h2>
<pre><code class='language-java' lang='java'>package com.example.class_test;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.View;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

}
</code></pre>
<p> </p>
<p>其他布局文件请查看源代码</p>
</body>
</html>
