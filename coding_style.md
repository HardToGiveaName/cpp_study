# C++ Coding Style
1. 变量、函数名、命名空间 使用 snake case , 全局变量前加 `g_` 前缀
2. 自定义类名用 Camel Case, 成员函数用 snake case, 成员变量前加 `m_` 前缀
3. 宏和常量用大写, 单词间用下划线连接

```c++

#define MAX_PATH_LEN 256     /* 宏大写, _相连 */

int g_sys_flag;              /* 全局变量前缀 g_ */

namespace linux_sys {        /* 命名空间, snake case */
    void get_rlimit_core();  /* 函数, snake case */
}

class FilePath final         /* 自定义类名, Camel Case */
{
public:
    void set_path(const string& str); /* 成员函数, snake case */
private:
    string m_path;           /* 类成员, 前加 _m */
    int m_level;
};

```
