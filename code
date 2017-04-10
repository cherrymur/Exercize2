// в функцию добавлена переменная n для контроля длины вводимого массива.
#include <iostream>
#include <cmath>
#include <vector>
using namespace std;

int task1(vector<int>&nums, int k, int n) {
	//ввод одномерного массива
	for (int i = 0; i < n; i++) {
		cin >> nums[i];
	}
	// сортировка
	for (int j = 0; j < n; j++) {
		int max = nums[j];
		for (int i = j; i < n; i++) {
			if (nums[i] > max) {
				max = nums[i];//максимальный элемент
			}
		}
		for (int i = j; i < n; i++) {
			if (nums[i] == max) {
				int temp = max;
				nums[i] = nums[j];
				nums[j] = max;
			}
		}
	}
	return nums[k - 1];
}
	//вывод
int main() {
	int k;
	cin >> k;
	int n;
	cin >> n;
	vector<int>nums (n);
	cout << task1(nums, k, n);
	return 0;
}
