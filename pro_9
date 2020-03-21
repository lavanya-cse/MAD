package com.example.exno10; 

importandroid.app.Notification; 
importandroid.app.NotificationManager; 
importandroid.app.PendingIntent; 
importandroid.content.Intent; 
importandroid.os.Bundle;
importandroid.support.v7.app.AppCompatActivity; 
importandroid.view.View; 
importandroid.widget.Button; 
importandroid.widget.EditText; 
 
public class MainActivity extends AppCompatActivity  
{     
	Button notify;     
	EditText e;     
	@Override     
	protected void onCreate(Bundle savedInstanceState)      
	{ 
		super.onCreate(savedInstanceState); 
		setContentView(R.layout.activity_main); 
 		notify= (Button) findViewById(R.id.button);         
		e= (EditText) findViewById(R.id.editText); 
 		notify.setOnClickListener(newView.OnClickListener()         
		{             
			@Override             
			PublicvoidonClick(View v)              
			{                 
				Intent intent = newIntent(MainActivity.this, SecondActivity.class);                 
				PendingIntent pending = PendingIntent.getActivity(MainActivity.this, 0, intent, 0); 
				Notification noti = newNotification.Builder(MainActivity.this).setContentTitle("New Message").setContentText(e.getText().toString()).setSmallIcon(R.mipmap.ic_launcher).setCont entIntent(pending).build();                 
				NotificationManager manager = (NotificationManager) getSystemService(NOTIFICATION_SERVICE);                 
				noti.flags |= Notification.FLAG_AUTO_CANCEL; manager.notify(0, noti);             
			}         
		});     
	} 
} 
