<h1 align='center'>Linear Search and Binary Search written in C++</h1>

<h2>Linear search</h2>

```c++
int lsearch(int a[], int v, int l, int r)

{

for (int i=l; i<=n; i++)

if (v==a[i]) return i;

return -1;

}

```


<h2>Binary Search</h2>

```c++
int bsearch(int a[], int v, int l, int n)

{

while (r>=l)

{int m=(l+r)/2;

if (v==a[m]) return m;

if (v<a[m]) r=m-1; else l=m+1;

}

return -1;

}
```
