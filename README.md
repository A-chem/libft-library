# libft-library

---
Libft is a foundational project at 42 that consists of re-implementing many standard C library functions such as memset, strcpy, atoi, isdigit, and more, entirely from scratch. It focuses on mastering low-level memory manipulation, pointer arithmetic, and writing clean, efficient, and reusable C code. The project also includes a bonus section to implement a full set of linked list utilities. Libft lays the groundwork for all future C projects at 42 by teaching essential skills like modular programming, memory safety, and Makefile usage.

````markdown
# 📚 Libft – Your First C Library

> 🛠️ A foundational project at 42 that teaches you how to re-create common C standard library functions from scratch.  
> 📘 Built entirely in C with strict memory and style rules.

---

## 📌 Project Description

Libft is a personal library of functions written in C. It includes re-implementations of standard libc functions as well as additional utilities to simplify C programming.

You will use this library in many future 42 projects (like `get_next_line`, `ft_printf`, `push_swap`, `pipex`, and more).

---

## 🧠 What You’ll Learn

- How the standard C library works internally  
- String, memory, and character manipulation  
- Dynamic memory allocation  
- Function pointers and advanced manipulation  
- Working with singly linked lists  
- Writing and organizing modular C code  
- Creating a static library using `ar`

---

## 🧾 Contents

The project is divided into three main parts:

1. **Mandatory Libc functions**
2. **Additional utility functions**
3. **Bonus – Linked list operations**

---

## 🔹 Mandatory Part

### 🧪 Part 1: Re-implementation of libc functions

You must rewrite the following standard C functions with a `ft_` prefix:

| Category       | Functions                                                                 |
|----------------|--------------------------------------------------------------------------|
| Character check| `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`     |
| Memory         | `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`, `ft_memchr`, `ft_memcmp` |
| Strings        | `ft_strlen`, `ft_strlcpy`, `ft_strlcat`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`, `ft_strnstr`, `ft_strdup` |
| Conversion     | `ft_toupper`, `ft_tolower`, `ft_atoi`                                     |
| Allocation     | `ft_calloc`                                                               |

Each function must behave identically to its libc counterpart but without relying on the real implementation.

---

### 🔹 Part 2: Additional Utility Functions

| Function       | Description                                                              |
|----------------|--------------------------------------------------------------------------|
| `ft_substr`    | Extracts a substring from a string                                       |
| `ft_strjoin`   | Joins two strings into a new one                                         |
| `ft_strtrim`   | Trims characters from the start and end of a string                      |
| `ft_split`     | Splits a string into an array by a delimiter                            |
| `ft_itoa`      | Converts an integer to a string                                          |
| `ft_strmapi`   | Applies a function to each character (returns a new string)             |
| `ft_striteri`  | Applies a function to each character (in-place modification)            |
| `ft_putchar_fd`| Outputs a character to a given file descriptor                          |
| `ft_putstr_fd` | Outputs a string to a given file descriptor                             |
| `ft_putendl_fd`| Outputs a string + newline to a file descriptor                         |
| `ft_putnbr_fd` | Outputs a number to a file descriptor                                   |

---

## 🌟 Bonus Part (Optional)

### 🧩 Linked List Functions

If you complete all mandatory functions **perfectly**, you may implement:

```c
typedef struct s_list
{
    void *content;
    struct s_list *next;
} t_list;
````

| Function          | Description                                           |
| ----------------- | ----------------------------------------------------- |
| `ft_lstnew`       | Create a new node                                     |
| `ft_lstadd_front` | Add a node to the front of the list                   |
| `ft_lstadd_back`  | Add a node to the end of the list                     |
| `ft_lstsize`      | Count the number of nodes                             |
| `ft_lstlast`      | Return the last node                                  |
| `ft_lstdelone`    | Free a node using a custom delete function            |
| `ft_lstclear`     | Clear the whole list                                  |
| `ft_lstiter`      | Apply a function to each node’s content               |
| `ft_lstmap`       | Create a new list by applying a function to each node |

📝 These must go in separate `_bonus.c` and `_bonus.h` files and be built with the `bonus` Makefile rule.

---

## 🛠️ Makefile

Your `Makefile` must include the following rules:

* `all`: builds the library
* `clean`: removes object files
* `fclean`: removes object files and the library
* `re`: re-compiles everything
* `bonus`: builds with bonus list functions

Use:

```bash
make
make bonus
```

---

## 🧪 Testing

Although tests are not required, it is **highly recommended** to write your own:

* Test each function against the original libc version
* Compare return values, memory output, and behavior on edge cases
* Use tools like `valgrind` to check for leaks

---

## 📁 Project Structure

```txt
libft/
├── ft_*.c             # All your function implementations
├── ft_*.h             # (optional) additional headers if needed
├── libft.h            # Main header file with all prototypes
├── Makefile           # Builds libft.a
├── libft.a            # Final static library (after make)
└── README.md          # This file
```

---

## ✅ Rules & Requirements

* ❌ No global variables
* ✅ Follow 42 Norme
* ❌ No libtool or external libraries
* ✅ Compile with `-Wall -Wextra -Werror`
* ✅ All memory must be freed
* ❌ No undefined behavior or crashes

---

## 👨‍💻 Author

🧑‍💻 [Abdilah Chemlal](https://github.com/A-chem)

---

## 🏁 License

This project is part of the 42 school curriculum.
Do not submit or share full solutions. Use this only for learning and testing purposes.

---



