# Clipboard API
A simple wrapper around different APIs for fetching and setting clipboard content.

Currently only supported in Windows, want to add support Mac and Linux later.

# Example Usage
```c
#include "clipboard.h"
#include <stdio.h>

int main()
{
    set_clipboard_content("hello there");

    char* content = NULL;
    get_clipboard_content(&content);

    printf("%s\n", content);
    free(content);
    
    return 0;
}
```