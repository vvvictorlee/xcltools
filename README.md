xcltools
========
 ��Golangд��һЩС������
 
cdir  ��ʾ��ǰ����Ŀ¼����.
OPTIONS:
  -h=false: ��ʾ���������Ϣ
  -a="": ����ʾָ��ʱ��(��:2014-10-10_21:14:25)֮����ļ���Ŀ¼.
  -b="": ����ʾָ��ʱ��(��:2014-10-10_21:14:25)֮ǰ���ļ���Ŀ¼.
  -e="": ָ�����ų���ָ����չ���ļ�(��:.bak|.dbf).
  -i="": ������ָ����չ�����ļ�(��:.log|.ora),�����������ȫ��.
  -d=true: �Ƿ���ʾĿ¼.
  -f=true: �Ƿ���ʾ�ļ�.
  -s=true: �Ƿ���ʾ�ļ���С.
  -t=true: �Ƿ���ʾʱ��.
  -tr=true: �Ƿ������η�ʽ��ʾ�ļ���Ŀ¼.
  -fu=false: �Ƿ���ȫ·����ʽ��ʾ�ļ���Ŀ¼.
EXAMPLE:
  cdir -h
  ./cdir /usr/local/go
  cdir -f=false c:\go\doc
  ./cdir -s=false  /u01/oracle/oradata/xcldb/archivelog -a=2012-11-18_14:27:04
  ./cdir -d=false -fu=true -t=false -e=.out|.go|.jpg|.png /usr/local/go/doc
  
  
NAME:
  scounter <options> <path> ͳ�ƴ�������
OPTIONS:
  -i="": ������ָ����չ�����ļ�(��:.java,.cpp,.h),�����������ȫ��.
  -v=false: �Ƿ���ʾ�ļ�ͳ����ϸ.
  -l=0: ��ͳ�ƽ�����г����ڵ�����ָ������(0Ϊ����¼)���ļ���Ϣ.
EXAMPLE:
  scounter -i .java c:\xclcharts\xclcharts\src
  scounter -i=.cpp,.h,.hpp,.c /xclproject/src
  scounter -i .go -v=false /usr/local/go/src
  scounter -l=680 -i=.cpp,.h,.hpp,.c  /xclproject/common/src
  
  
����ͳ�ƻ���(2014-12-22 22:20:47)
=================================================
������Ŀ¼: E:\GitHub\GitHub\XCL-Charts\XCL-Charts\src

 ��������     : �ļ�����
-------------------------------------------------
 line <= 300  : 92
 line <= 500  : 13
 line <= 1000 : 6
 line <= 5000 : 0
 line > 5000  : 0
-------------------------------------------------
 �������ܼ�: 18214  ע�����ܼ�: 7068
 �����ļ���: 111

������( >= 600 )�ļ���ϸ:
   ������    ע����    �ļ���
-------------------------------------------------
   987         154    .\org\xclcharts\renderer\AxesChart.java
   620          53    .\org\xclcharts\chart\AreaChart.java
   615          27    .\org\xclcharts\renderer\plot\PlotLegendRender.java
   610          97    .\org\xclcharts\chart\BarChart.java
-------------------------------------------------
             �ļ���:4

elapsed 1.744222 seconds  