# Development of Lianliankan game based on Python
基于Python的连连看游戏开发  

public partial class Form1:Form
  {MapMode myMapMode; Rule myRule; Draw myDraw;
      boot GameStart = false;//是否开始游戏
    int clickSum = 0;//记录点击图片的次数最大为2
      public Point fpoint;//记录第一次点击的位置
      public Point spoint;//记录第二次点击的位置
      int pbvalue = 100;//processbar进度条的值
      public Form1()
      {InitializeComponentU;}
      //点击’‘开始”按键的响应事件
      private void btnStart_ Click(object sender, EventArgs e)
      {if (GameStart==false)
        {myMapMode=new MapMode(18, 4);
          myRule=new Rule(ref myMapMode.gmap);
          myDraw=new Draw(pictureBox1);
            GameStart=true;
            myDraw.label=label2;
            pbvalue=100;
          myDraw.BackgroundClear();
            //画图
          for (int i=0; i<myMapMode.mapwidth; i++)
              for (int]=0;]<myMapMode.mapheight;]++)
              {if (myMapMode.gmap[i,]」!=0)
                  {myDraw.Drawlmage (myMapMode.img
[myMapMode.gmap   [i]」」i  *  myMapMode.picwidth]
myMapMode.picheight);
                  }
                }
            timer1.StartU;
          }
