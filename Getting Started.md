一、开始
这个章节主要是介绍一些关于如何使用MPAndroidChart库的基本概念。

1.添加依赖
  第一步首先在Android Studio中，添加dependency到你的项目中。如何添加dependency到自己项目中，参见repository usage（https://github.com/PhilJay/MPAndroidChart#usage）说明
  目前建议是用Gradle添加依赖使用这个图库。
2.新建一个View
  对于应用 LineChart, BarChart, ScatterChart, CandleStickChart, PieChart, BubbleChart or RadarChart ,可以直接添加到XML文件中，如下：
      <com.github.mikephil.charting.charts.LineChart
        android:id="@+id/chart"
        android:layout_width="match_parent"
        android:layout_height="match_parent" />
  And then retrieve it from your Activity, Fragment or whatever:
  然后可以在Activity 和Fragment或这是其他父控价中国呢获取，如下：
    // 在这个例子中, 一个 LineChart 被从XML文件初始化。
    LineChart chart = (LineChart) findViewById(R.id.chart); 
  我们也可以直接在Code中新建，并添加到布局中，
  
