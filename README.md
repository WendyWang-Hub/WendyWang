# Hello😊 I'm WendyWang
**Im a first-year student majoring in Digital Media Technology**😝

I enjoy art and games,and I've also been studying game engines and development.I hope to leverage my strengths through learning.

___________________________________________________________________

## About me🎶
My Chinese name🐳:王轩仪

My English name🎈:Wendy

Sure,you can also call me by my online name"Arlene",isn't it very trendy?🦸‍♀️

______________________________________________

## Interests😍
**Game engine**🩵

**3D modeling**🩷

**Graphic design**💚

________________________________________________

## Current skills🍔
**C#** 🍕:(Actually,I only know a bit about this aspect.....)

**PS/Sai**🌭:Use PS for painting and photo editing.Use Sai for creating design.

**Maya/3Ds max/zbrush**🍿:I use maya for character and scence modeeling.Then use Zb to crave the model.Use 3Ds max for character bone binding and animation production.

____________________________________________

## Currently Learning🎉
**Code writing and game engine development**✨:I'm very interested in developing and making games,but I'm just a novice when it comes to writing code.

**Scene original art and character design**🎊:Painting is my hobby,so I haven't stopped at illustration but hope to engage in original art design.

**3D animation**🎁:I self-studied 3D skeletal binding and animation.

__________________________________________________

## What I want to build✈️
**A complete game scene**🪂

**Some characters that can move in the scene**🛞

**Some physical effects that can be fully presented**🌍

______________________________________________________

## Preferred role👩‍💻
**Technical Artist/Artist**🧚‍♀️

_____________________________________________________

## Strengths☪️
**Painting and design**🕎

__________________________________________

## Contact🏯
**Mailbox**🏞️:xuantang6014278537@163.com

**Wechat**🏖️:W13651164058

____________________________________________

## Other😶‍🌫️
I'm rather confused about the direction I want to choose in the future.Maybe it's scene design,animation production or TA.

——————————————————————————————————————————————

# 冒泡排序
**（发的word我自己没打开，不知道是否能打开，因此在这里也写一下）**

#include <iostream>

using namespace std;

int main() {

    int arr[] = {8, 3, 6, 2, 7, 1};
    
    int n = 6

    // 排序
    
    for (int i = 0; i < n - 1; i++) {
    
        for (int j = 0; j < n - 1 - i; j++) {
        
            // 如果前一个数比后一个数大则交换它们的位置
            
            if (arr[j] > arr[j + 1]) {
            
                int temp = arr[j];
                
                arr[j] = arr[j + 1];
                
                arr[j + 1] = temp;
                
            }
            
        }
        
    }

    // 输出结果
    
    cout << "从小到大排序后的结果: ";
    
    for (int i = 0; i < n; i++) {
    
        cout << arr[i] << " ";
        
    }
    
    cout << endl;

    return 0;
    
}

1. 你的程序是如何完成排序的？

使用双重循环。外层循环控制排序的轮数，共比较 n-1 轮。内层循环在每一轮从左到右比较相邻的两个数字。如果发现左边的数字大于右边的数字就把他俩交换位置。每完成一轮内层循环未排序部分中最大的数字就会被拍到最后面。反复几轮就从小到大排好序了。

2. 冒泡排序的基本思路是什么？

重复走访要排序的数列，每一次比较两个相邻的元素，若出现错误如从小到大排列，出现后一个数比前一个数小，就交换。重复地进行直到没有再需要交换，则排序完成。

3. 如果要改成从大到小排序，需要修改哪里？
   
内层循环中的判断条件：
if (arr[j] > arr[j + 1]) 修改为 if (arr[j] < arr[j + 1])。


