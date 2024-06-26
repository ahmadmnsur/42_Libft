![42 beirut](https://media.licdn.com/dms/image/D4E3DAQGxvimpQQFi_A/image-scale_191_1128/0/1695893480399/42_beirut_cover?e=2147483647&v=beta&t=oNrMR2IXjtfu3XXV-uSUW8wI98g19yUUHZ0XuhtX2NE)

<h2>Overview</h2>
<p>The Libft project is a core and essential part of the 42 curriculum, centered on creating a custom C library. In this project, students are required to implement a set of standard library functions from scratch, laying a strong foundation for future programming tasks. This project provides an in-depth introduction to C programming, memory management, and code organization.</p>

<h2><b>Libc functions</b></h2>

<p align="left̨">
 
|Function|Description|
|:-------|:----------|
isalpha |checks if a character is an alphabetic character (a letter).
isdigit |checks if a character is a digit (0-9).
isalnum | checks if a character is alphanumeric (a letter or a digit).
isascii | checks if a character is a valid ASCII character (0-127 range).
isprint | checks if a character is printable (including spaces and printable ASCII characters).
strlen | calculates the length of a null-terminated string (excluding the null terminator).
memset | sets a block of memory to a specified value.
bzero | sets a block of memory to zero.
memcpy | copies a block of memory from one location to another.
memmove | moves a block of memory, handling overlapping regions correctly.
strlcpy | copies a string into a destination buffer with a specified size, ensuring null-termination.
strlcat | appends a string to the end of a destination string, ensuring the result is null-terminated and fits within a specified size.
toupper | converts a lowercase character to uppercase if applicable, otherwise it returns the same character.
tolower | converts an uppercase character to lowercase if applicable, otherwise it returns the same character.
strchr | searches for the first occurrence of a specified character within a string and returns a pointer to it.
strrchr | searches for the last occurance of a specified character within a string and returns a pointer to it.
stnrcmp | compares two strings up to a specified number of characters and returns the comparison result.
memchr | searches for the first occurrence of a specified byte value within a memory block and returns a pointer to it.
memcmp | compares two memory blocks up to a specified number of bytes and returns the comaprison result.
strnstr | searches for the first occurrence of a substring within a string, up to a specified number of characters.
atoi | converts a string to an integer, discarding leading whitespace and stopping at the first non-digit character.
calloc | allocates and initializes a block of memory for an array, setting all bytes to zero.
strdup | creates a new string by duplicating an existing null-terminated string and returns a pointer to it.

---


|Function name        |ft_substr|
|:--------------------|:--------|
|Prototype|char *ft_substr(char const *s, unsigned int start, size_t len);|
|Turn in files|-|
|Parameters|<b>s</b>: The string from which to create the substring. <b>start</b>: The start index of the substring in the string ’s’. <b>len</b>: The maximum length of the substring.|
|Return value|The substring. NULL if the allocation fails.|
|External ft.|malloc|
|Description|Allocates (with malloc(3)) and returns a substring from the string ’s’. The substring begins at index ’start’ and is of maximum size ’len’.|


|Function name        |ft_strjoin|
|:--------------------|:--------|
|Prototype|char *ft_strjoin(char const *s1, char const *s2);|
|Turn in files|-|
|Parameters|<b>s1</b>: The prefix string. <b>s2</b>: The suffix string.|
|Return value|The new string. NULL if the allocation fails.|
|External ft.|malloc|
|Description|Allocates (with malloc(3)) and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’.|


|Function name        |ft_strtrim|
|:--------------------|:--------|
|Prototype|char *ft_strtrim(char const *s1, char const *set);|
|Turn in files|-|
|Parameters|<b>s1</b>: The string to be trimmed. <b>set</b>: The reference set of characters to trim.|
|Return value|The trimmed string. NULL if the allocation fails.|
|External ft.|malloc|
|Description|Allocates (with malloc(3)) and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string.|


|Function name        |ft_split|
|:--------------------|:--------|
|Prototype|char **ft_split(char const *s, char c);|
|Turn in files|-|
|Parameters|<b>s</b>: The string to be split. <b>s2</b>: The delimiter character.
|Return value|The array of new strings resulting from the split. NULL if the allocation fails.|
|External ft.|malloc, free|
|Description|Allocates (with malloc(3)) and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter. The array must end with a NULL pointer.|


|Function name        |ft_itoa|
|:--------------------|:--------|
|Prototype |char *ft_itoa(int n);|
|Turn in files|-|
|Parameters|<b>n</b>: The integer to convert.|
|Return value|The string representing the intege. NULL if the allocation fails.|
|External ft.|malloc|
|Description|Allocates (with malloc(3)) and returns a string representing the integer received as an argument. Negative numbers must be handled.|


|Function name        |ft_strmapi|
|:--------------------|:--------|
|Prototype|char *ft_strmapi(char const *s, char (*f)(unsigned int, char));|
|Turn in files|-|
|Parameters|<b>s</b>: The string on which to iterate. <b>f</b>: The function to apply to each character.|
|Return value|The string created from the successive applications of ’f’. NULL if the allocation fails.|
|External ft.|malloc|
|Description|Applies the function ’f’ to each character of the string ’s’, and passing its index as first argument to create a new string (with malloc(3)) resulting from successive applications of ’f’.|


|Function name        |ft_striteri|
|:--------------------|:--------|
|Prototype |void ft_striteri(char *s, void (*f)(unsigned int, char *);|
|Turn in files|-|
|Parameters|<b>s</b>: The string on which to iterate. <b>f</b>: The function to apply to each character.|
|Return value|None|
|External ft.|None|
|Description|Applies the function ’f’ on each character of the string passed as argument, passing its index as first argument. Each character is passed by address to ’f’ to be modified if necessary.|


|Function name        |ft_putchar_fd|
|:--------------------|:--------|
|Prototype |void ft_putchar_fd(char c, int fd);|
|Turn in files|-|
|Parameters|<b>c</b>: The character to output. <b>fd</b>: The file descriptor on which to write.|
|Return value|None|
|External ft.|write|
|Description|Outputs the character ’c’ to the given file descriptor.|


|Function name        |ft_putstr_fd|
|:--------------------|:--------|
|Prototype |void ft_putstr_fd(char *s, int fd);|
|Turn in files|-|
|Parameters|<b>s</b>: The string to output. <b>fd</b>: The file descriptor on which to write.|
|Return value|None|
|External ft.|write|
|Description|Outputs the string ’s’ to the given file descriptor.|


|Function name        |ft_putendl_fd|
|:--------------------|:--------|
|Prototype |void ft_putendl_fd(char *s, int fd);|
|Turn in files|-|
|Parameters|<b>s</b>: The string to output. <b>fd</b>: The file descriptor on which to write.|
|Return value|None|
|External ft.|write|
|Description|Outputs the string ’s’ to the given file descriptor followed by a newline.|


|Function name        |ft_putnbr_fd|
|:--------------------|:--------|
|Prototype |void ft_putnbr_fd(int n, int fd);|
|Turn in files|-|
|Parameters|<b>n</b>: The integer to output. <b>fd</b>: The file descriptor on which to write.|
|Return value|None|
|External ft.|write|
|Description|Outputs the integer ’n’ to the given file descriptor.|

<h2><b>¤ Bonus functions ¤</b></h2>

|Function name	|ft_lstnew|
|:--------------------|:--------|
|Prototype	t_list| *ft_lstnew(void *content);|
|Turn in files|-|
|Parameters	content:| The content to create the node with.|
|Return value|	The new node|
|External ft.|	malloc|
|Description|	Allocates (with malloc(3)) and returns a new node. The member variable content is initialized with the value of the parameter content. The variable next is initialized to NULL.|

|Function name|	ft_lstadd_front|
|:--------------------|:--------|
|Prototype|	void ft_lstadd_front(t_list **lst, t_list *new);|
|Turn in files|-|
|Parameters|	<b>lst</b>: The address of a pointer to the first link of a list. <br> <b>new<b>: The address of a pointer to the node to be added to the list.|
|Return value|None|
|External ft.|None|
|Description|	Adds the node new at the beginning of the list pointed to by lst.|

|Function name|	ft_lstsize|
|:--------------------|:--------|
|Prototype|	int ft_lstsize(t_list *lst);|
|Turn in|files|-|
|Parameters|	<b>lst<b>: The beginning of the list.|
|Return value|	The length of the list|
|External ft.|	None|
|Description|	Counts the number of nodes in a list.|

|Function name|	ft_lstlast|
|:--------------------|:--------|
|Prototype|	t_list *ft_lstlast(t_list *lst);|
|Turn in files|-|
|Parameters|	<b>lst</b>: The beginning of the list.|
|Return value|	Last node of the list|
|External ft.|None|
|Description|	Returns the last node of the list. If the list is empty (lst is NULL), returns NULL.|

|Function name|	ft_lstadd_back|
|:--------------------|:--------|
|Prototype|	void ft_lstadd_back(t_list **lst, t_list *new);|
|Turn in files|-|
|Parameters| <b>lst</b>: The address of a pointer to the first link of a list. <br> <b>new</b>: The address of a pointer to the node to be added to the list.|
|Return value|None|
|External ft.|None|
|Description|	Adds the node new at the end of the list pointed to by lst. If lst is NULL, the function initializes the list with new as the first node.|

|Function name|	ft_lstdelone|
|:--------------------|:--------|
|Prototype|	void ft_lstdelone(t_list *lst, void (*del)(void *));|
|Turn in files|-|
|Parameters|	<b>lst</b>: The node to free. <br> <b>del</b>: The address of the function used to delete the content.|
|Return value|None|
|External ft.|free|
|Description	|Takes as a parameter a node lst and frees the memory of the node’s content using the function del given as a parameter, and then frees the node itself. The memory of the next pointer must not be freed.|

|Function name	|ft_lstclear|
|:--------------------|:--------|
|Prototype|	void ft_lstclear(t_list **lst, void (*del)(void *));|
|Turn in files|-|
|Parameters|	<b>lst</b>: The address of a pointer to a node. <br> <b>del</b>: The address of the function used to delete the content of the node.|
|Return value|None|
|External ft.|free|
|Description| Deletes and frees the given node and every successor of that node, using the function del to delete the content of each node and free(3) to free the memory. Finally, sets the pointer to the list (lst) to NULL.|

|Function name|	ft_lstiter|
|:--------------------|:--------|
|Prototype|	void ft_lstiter(t_list *lst, void (*f)(void *));|
|Turn in files|-|
|Parameters|	<b>lst</b>: The address of a pointer to a node. <br> <b>f</b>: The address of the function used to iterate on the list.|
|Return value|None|
|External ft.|None|
|Description| Iterates through the list lst and applies the function f to the content of each node. The function f should take a void * parameter representing the content of the node.|

|Function name|	ft_lstmap|
|:--------------------|:--------|
|Prototype| t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));|
|Turn in files|-|
|Parameters| <b>lst</b>: The address of a pointer to a node. <br> <b>f</b>: The address of the function used to iterate on the list. <br> <b>del</b>: The address of the function used to delete the content of a node if needed.|
|Return value|	The new list. NULL if the allocation fails.|
|External ft.|	malloc, free|
|Description|	Iterates through the list lst and applies the function f to the content of each node. Creates a new list resulting from the successive applications of the function f. The del function is used to delete the content of a node if needed (e.g., during error handling or cleanup). Returns a pointer to the new list. If memory allocation fails during the creation of the new list, returns NULL.|

---
