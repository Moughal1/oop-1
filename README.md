# oop-1
Assignment
#include<iostream.h>
#include<conio.h>
class Distance
{
private :
int foot, inch;
public:
Distance(): foot (0), inch(0) { }
Distance(int f ,int in ) : foot (f), inch (in) {}
void getdist()
{
cout <<"\nenter foot :"; cin >> foot;
cout <<"enter inch :";  cin >> inch;
}
void showdist()
{ 
cout << foot <<"-"<<inch << endl;}
void sub_dist(Distance,Distance);
};
void Distance::sub_dist(Distance d2, Distance d3)

{
if{d2.inch<d3.inch||d2.foot<d3.foot)
{
cout<<"the value of d2 is smaller than d3 so it can'tbe subtracted";
}
else
{
inch =d2.inch-d3.inch;
foot=0;
{
feet --;
}
foot -=d2.foot-d3.foot;
}

int main ()
{
Distance dist1,dist3;
dist1.showdist();
dist3.showdist();
Distance dist2(10,3);
dist2.showdist();
dist1.getdist();
dist3.sub_dist(dist1,dist2);
cout<<"\n dist1 = ";
dist1.showdist();
cout<<"\n dist2 = ";
dist2.showdsit();
cout<<"\ndist3 = ";
dist3.showdist();
cout <<endl;
return 0;
}
