package com.example.calculator_p2;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.text.TextUtils;
import android.view.View;
import android.view.View.OnClickListener;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity implements OnClickListener
{
    EditText Num1;
    EditText Num2;
    Button Add;
    Button Sub;
    Button Mul;
    Button Div;
    TextView Result;

    @Override
    public void onCreate(Bundle savedInstanceSate)
    {
        super.onCreate(savedInstanceSate);
        setContentView(R.layout.activity_main);

        Num1=(EditText)findViewById(R.id.editText3);
        Num2=(EditText)findViewById(R.id.editText4);
        Add=(Button)findViewById(R.id.button);
        Sub=(Button)findViewById(R.id.button2);
        Mul=(Button)findViewById(R.id.button3);
        Div=(Button)findViewById(R.id.button4);
        Result=(TextView)findViewById(R.id.textView2);

        Add.setOnClickListener(this);
        Sub.setOnClickListener(this);
        Mul.setOnClickListener(this);
        Div.setOnClickListener(this);
    }
    @Override
    public  void  onClick(View v)
    {
        float num1=0;
        float num2=0;
        float result=0;
        String oper="";

        if(TextUtils.isEmpty(Num1.getText().toString())|| TextUtils.isEmpty(Num2.getText().toString()))
            return;

        num1=Float.parseFloat(Num1.getText().toString());
        num2=Float.parseFloat(Num2.getText().toString());

        switch(v.getId())
        {
            case R.id.button:
                oper="+";
                result=num1+num2;
                break;

            case R.id.button2:
                oper="-";
                result=num1-num2;
                break;

            case R.id.button3:
                oper="*";
                result=num1*num2;
                break;

            case R.id.button4:
                oper="/";
                result=num1/num2;
                break;
        }
        Result.setText("num1 "+num1+" "+oper+"num2 "+num2+" = "+result);
    }
}
