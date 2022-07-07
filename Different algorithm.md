<h2 align = "Center">Algorithms</h2>
<h3 align = "Center">Convex hull Problem -Algorithm</h3>

```
vector<pair<int, int>> divide(vector<pair<int, int>> a)

{

  if (a.size() <= 5)

    return bruteHull(a);

  vector<pair<int, int>>left, right;

  for (int i=0; i<a.size()/2; i++)

  left.push_back(a[i]);

  for (int i=a.size()/2; i<a.size(); i++)

  right.push_back(a[i]);

    vector<pair<int, int>>left_hull = divide(left);

  vector<pair<int, int>>right_hull = divide(right);

  return merger(left_hull, right_hull);

  }

```

<h3 align="Center">Finding Minimum and Maximum</h3>

```
Algorithm MaxMin(A, n, max, min)// DIRECT APPROACH
// Set max to the maximum and min to the minimum of A[1..n]
{
max = min = A[1];
for( i = 2 to n ) do
{
if (A[i]>max) then max = A[i];
if (A[i]<min) then min = A[i];
}
}
```

