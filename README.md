# tia#include <conio.h>
#include <iostream.h>

int a[10][10], b[10][10], c[10][10];
void nhap(char, int, int);
void xuat(char, int, int);
void nhan(int, int, int);

void main()
{
	int m, n, p;
	clrscr();
	cout << "Nhap kich thuoc mang a: so hang, so cot<10, so hang m=";
	cin >> m;
	cout << "so cot n=";
	cin >> n;
	cout << "Nhap kich thuoc mang b: so hang = so cot mang a la " << n << ", so cot<10, so cot p=";
	cin >> p;
	cout << "Nhap mang a :\n";
	nhap('a', m, n);
	cout << "Nhap mang b :\n";
	nhap('b', n, p);
	cout << "\nMang A :\n";
	xuat('a', m, n);
	cout << "\n\nMang B :\n";
	xuat('b', n, p);
	nhan(m, n, p);
	cout << "\n\nMang C=AxB:\n";
	xuat('c', m, p);
}

void nhap(char k, int p, int q)
{
	int i, j, t;
	for (i = 0; i < p; i++)
	{
		cout << "Nhap cac phan tu hang thu " << i + 1 << ":\n";
		for (j = 0; j < q; j++)
		{
			cout << k << "[" << i + 1 << "," << j + 1 << "]=";
			cin >> t;
			switch (k)
			{
				case 'a':
					a[i][j] = t;
					break;
				case 'b':
					b[i][j] = t;
			}
		}
	}
}

void xuat(char k, int p, int q)
{
	int i, j;
	for (i = 0; i < p; i++)
	{
		cout << endl;
		for (j = 0; j < q; j++)
		{
			cout << " ";
			switch (k)
			{

void nhan(int m, int n, int p)
{
	int i, j, k, s;#include <conio.h>
#include <iostream.h>

int a[10][10], b[10][10], c[10][10];
void nhap(char, int, int);
void xuat(char, int, int);
void nhan(int, int, int);

void main()
{
	int m, n, p;
	clrscr();
	cout << "Nhap kich thuoc mang a: so hang, so cot<10, so hang m=";
	cin >> m;
	cout << "so cot n=";
	cin >> n;
	cout << "Nhap kich thuoc mang b: so hang = so cot mang a la " << n << ", so cot<10, so cot p=";
	cin >> p;
	cout << "Nhap mang a :\n";
	nhap('a', m, n);
	cout << "Nhap mang b :\n";
	nhap('b', n, p);
	cout << "\nMang A :\n";
	xuat('a', m, n);
	cout << "\n\nMang B :\n";
	xuat('b', n, p);
	nhan(m, n, p);
	cout << "\n\nMang C=AxB:\n";
	xuat('c', m, p);
}

void nhap(char k, int p, int q)
{
	int i, j, t;
	for (i = 0; i < p; i++)
	{
		cout << "Nhap cac phan tu hang thu " << i + 1 << ":\n";
		for (j = 0; j < q; j++)
		{
			cout << k << "[" << i + 1 << "," << j + 1 << "]=";
			cin >> t;
			switch (k)
			{
				case 'a':
					a[i][j] = t;
					break;
				case 'b':
					b[i][j] = t;
			}
		}
	}
}

void xuat(char k, int p, int q)
{
	int i, j;
	for (i = 0; i < p; i++)
	{
		cout << endl;
		for (j = 0; j < q; j++)
		{
			cout << " ";
			switch (k)
			{
				case 'a':
					cout << a[i][j];
					break;
				case 'b':
					cout << b[i][j];
					break;
				case 'c':
					cout << c[i][j];
			}
		}
	}
}

void nhan(int m, int n, int p)
{
	int i, j, k, s;
	for (i = 0; i < m; i++)
		for (j = 0; j < p; j++)
		{
			for (k = s = 0; k < n; k++) s += a[i][k] *b[k][j];
			c[i][j] = s;
		}
}
			c[i][j] = s;
		}
}
