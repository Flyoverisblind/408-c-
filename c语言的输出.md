## c语言的输出

```c
#include <stdio.h>
int main()
{
	printf("hello，word");
	return 0;
}
```

## 输出计算结果

```c
printf("%d",1+2);
```

**%d表示整数，其余计算方式和其他语言一致**

## 变量和输入

```c
#include <stdio.h>
int main()
{
    //定义一个int类型的变量
	int a = 0;
    //在vs中使用scanf_s输入
	scanf_s("%d", &a);
	printf("%d",a);
	return 0;
}
```

**输入用scanf函数，在vs中用scanf_s，即scanf_s不能跨平台用**

**如果一定要使用scanf需要加上_CRT_SECURE_NO_WARNINGS**

```c
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
int main()
{
	//我是注释
	int a=6;
	scanf("%d", &a);
	printf("输入的是：%d", a);

	return 0;
}
```

**输入多个**

```c
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
int main()
{
	//我是注释
    int a, b;
    //输入的是10,20时中间加,
    scanf("%d,%d", &a, &b);
    scanf("%d %d", &a, &b);
    scanf("%d%d", &a, &b);
    printf("%d,%d",a,b);
	return 0;
}
```









