# GCD-
GREATEST COMMAN DIVISOR

#include <bits/stdc++.h>

using namespace std;

void gcd(int n, int m)
{
    cout << "Enter the number : " << endl;
    cin >> n >> m;
    int temp;
    if (n > 0 && m > 0)
    {
        if (n > m || n == m)
        {
            for (int i = 1; i <= n; i++)
            {
                if (n % i == 0 && m % i == 0)
                {
                    temp = i;
                    // cout<<temp<<" ";
                }
            }
        }
        else
        {
            for (int i = 1; i <= m; i++)
            {
                if (n % i == 0 && m % i == 0)
                {
                    temp = i;
                }
            }
        }
        cout << temp << " ";
        cout<<endl;
    }
}
int main()
{
    int a;
    cout << "Enter a test cases: " << endl;
    cin >> a;
    while (a > 0)
    {
        // string n, m;
        int n, m;
        // anagram(n, m);
        gcd(n, m);
        a--;
    }

    return 0;
}
