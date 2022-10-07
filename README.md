# library2
一.linerLayout
1.思路
  整个项目以linerlayout实现；
  因为页面有四行，所以在最大的linerlayout下再放入四个linerlayout
  因为每一行有四个text，所以在在每一个linerlayout下再放入四个textview
 
2.关键代码
<TextView
        android:id="@+id/textView"
        android:layout_width="83dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="16dp"
        android:background="@drawable/underline"
        android:text="One,One"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
        
3.页面显示
![BN3S}9BJS$4WQ$7N7HJ E8J](https://user-images.githubusercontent.com/114241292/194510901-db4dae7e-7b56-407a-b12b-95ecb04f842d.png)

二.tableLayout
1.思路
  整个项目以linerlayout实现
  因为页面有6行，所以在整个的tablelayout里写入六个TableRow
  再根据每一行的text个数xierutextview
 
 2.关键代码（此处以第一行为例）
 <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent" >

        <TextView
            android:id="@+id/textView2"
            android:layout_weight="1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Open..." />

        <TextView
            android:id="@+id/textView3"
            android:layout_weight="1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Ctrl-O"
            android:gravity="right"/>
    </TableRow>

3.页面显示
![~T4 Z~%2NG40X0CWU_K $ 7](https://user-images.githubusercontent.com/114241292/194511076-783b3bb9-000e-4e71-a60d-a0e4ca473858.png)

三.constraintLayout
1.思路
  整个项目以constraintlayout实现
  使用design设计页面
  首先运用辅助线，记下button的大体布局，然后再一行四个button成链
  其他行数依次执行
 
2.关键代码（此处以一个button和一个guideline为例）
<Button
        android:id="@+id/button3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="9"
        app:layout_constraintBottom_toBottomOf="@+id/button2"
        app:layout_constraintEnd_toStartOf="@+id/button4"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button2"
        app:layout_constraintTop_toTopOf="@+id/button2" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_percent="0.17" />

页面显示
![D4J740V1L17S4QI}W 215)5](https://user-images.githubusercontent.com/114241292/194511233-41bba7aa-2073-4f4f-a710-75d44f011fa5.png)

四.constraintLayout2
1.思路
  整个项目以constraintlayout实现
  使用design设计页面
  部件全部拖进来以后，最后根据位置建立约束。
 
2.页面显示
![}N3_DT)F~01)FYS7JCX J87](https://user-images.githubusercontent.com/114241292/194511318-ab892489-65e1-4978-80e1-ae90e4a592ec.png)
