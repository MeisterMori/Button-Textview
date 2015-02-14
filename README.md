package com.MeisterMori.Morteza.buttonandtextview;

import java.util.Date;
import android.os.Bundle;
import android.view.View;
import android.view.View.OnClickListener;
import android.widget.Button;
import android.widget.TextView;

public class ShowTime extends Activity {
	
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.ShowTime);
        
   Button btn_Show = (Button)findViewById(R.id.btn_Show);
    
    
    btn_Show.setOnClickListener(new OnClickListener() {
		
		@Override
		public void onClick(View v) {
			// TODO Auto-generated method stub
			
			TextView txt_Show = (TextView)findViewById(R.id.txt_Show);
			txt_Show.setText(new Date().toString());
			
		}
	});
    	
       
    }
    
}
