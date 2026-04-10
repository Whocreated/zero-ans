#include<bits/stdc++.h>
using namespace std;
int main() {
	int n;
	string s[9][5];
	for (int i = 0;i < 9;i++) {
		cin >> n;
		for (int j = 0;j < n;j++) {
			cin >> s[i][j];
		}
	}
	int f;
	cin >> f;
	vector<string> v;
	for (int i = 0;i < 5;i++) {
		for (int j = 0;j < 9;j++) {
			if (s[j][i] == "1B" or s[j][i] == "2B" or s[j][i] == "3B" or s[j][i] == "HR" or s[j][i] == "FO" or s[j][i] == "GO" or s[j][i] == "SO") {
				v.push_back(s[j][i]);
			}
		}
	}
	int out = 0, score = 0;
	bool one = 0, two = 0, three = 0;
	for (int i = 0;i < v.size();i++) {
		if (v[i] == "FO" or v[i] == "GO" or v[i] == "SO") {
			out++;
			if (out == f) {
				cout << score;
				return 0;
			}
			if (out % 3 == 0) {
				one = 0;
				two = 0;
				three = 0;
			}
		}
		if (v[i] == "1B") {
			if (three) {
				score++;
			}
			three = two;
			two = one;
			one = 1;
		}
		if (v[i] == "2B") {
			if (three) {
				score++;
			}
			if (two) {
				score++;
			}
			three = one;
			two = 1;
			one = 0;
		}
		if (v[i] == "3B") {
			if (three) {
				score++;
			}
			if (two) {
				score++;
			}
			if (one) {
				score++;
			}
			three = 1;
			two = 0;
			one = 0;
		}
		if (v[i] == "HR") {
			if (three) {
				score++;
			}
			if (two) {
				score++;
			}
			if (one) {
				score++;
			}
			score++;
			three = 0;
			two = 0;
			one = 0;
		}
	}

}
