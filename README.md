#include<iostream>
using namespace std;

class person
{
public:
	int m_a;
	int m_b;

public:
	/*person  operator+(person& a)
	{
		person cc;
		cc.m_a = m_a + a.m_a;
		cc.m_b = m_b + a.m_b;
		return cc;
	}*/


};
person operator+(person &a, person &b)
{
	person ccc;
	ccc.m_a = a.m_a + b.m_a;
	ccc.m_b = a.m_b + b.m_b;
	return ccc;
}

void text01()
{
	person a;
	a.m_a = 10;
	a.m_b = 20;
	person b;
	b.m_a = 10;
	b.m_b = 20;
	person c;
	c = a + b;
	cout << "c的m_a是" << c.m_a;



}
int main()
{

	text01();


	system("pause");
	return 0;
}

