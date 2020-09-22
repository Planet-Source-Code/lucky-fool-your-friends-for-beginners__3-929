<div align="center">

## Fool Your Friends \-\- for beginners


</div>

### Description

Make your friends think that their harddrive will be formatted. You print "Hit Q to quit:" and when they try to hit 'Q' a 'Y' pops up... Of course, we won't really format or anything. Vote if you enjoy the code :)

BTW, to really close the program you must hit ESC.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[\*LuckY\*](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/lucky.md)
**Level**          |Beginner
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/lucky-fool-your-friends-for-beginners__3-929/archive/master.zip)





### Source Code

```
#include <conio.h>
#include <iostream>
using namespace std;
int main() {
	cout << "Windows 98 Setup will now format your hard drive...\n"
		"You will lose all files and settings currently configured\n"
		"on this hard drive. If you do not want to format, it is\n"
		"strongly recommended that you cancel Windows 98 Setup...\n\n"
		"If you decide to cancel during format, type EXIT.\n\n"
		"Press any key to format, or press 'Q' to quit setup: ";
	int ch;
	ch = getch();
	cout << "Y\n\n\a\a\aNow formatting . . . \n\n";
	while ((ch = getch()))
		if (ch == 27)
			break;
		else
			cout << char(ch+12);
	return 0;
}
```

