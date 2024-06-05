CSS NOTES


CSS POSITIONS
Absolute:   apny parent k position k hissab s move kry ga and apni jagah gap nhe bnaye ga like baqi bachy uski jagah aa jaien gay 
Like  tu yeh p apny first parent ki position main e move kry ga
<div class=”containter”>
	<p style=”position:absolute;top:5px;”></p>
</div>

Relative: apni position k hissab s move kry ga. Like neexhy waly main woh ab jo uski jagh  whan s 5 px udhr ho jai ga bhawy jo b ho jai and apni jagah bar gap bna dy ga 
<div class=”containter”>
	<p style=”position:relative;top:5px;”></p>
</div>


Fixed: like ek cheez hmesha browser ki height k hissab s visible rhy gi ya us jagah par hogi like footer on the bottom on screen 
Like .footer{
position:fixed;
Bottom:5px}


Sticky : sticky is jab ap scroll krien tu woh cheez screen p chiapk jati like a menu bar .. woh b sath sath neechy move krta .. 
Jaisy neechy screen main right wali screen jab hm scroll krien gay tu woh jab sticky div s neechy guzrien gay tu woh hmary sath move kry ga jab uski position browser k top p aa jai




CSS Display
Inline: tasks as much as minum width it can mtlb jitna content utni width. Agla content sath aa sakta  
Block: takes the whole row.. Agla content ab new line par e aaye ga
Inline block: it’s same as inline but we can set width and height of that . what we cant give to inline
Flex:
Flex is 1 d either horizontal or vertical . depending upon its direction the main line goes in parallel with direction and other one goes perpendicular 
https://css-tricks.com/snippets/css/a-guide-to-flexbox/
Grid: 
Grid is 2d, kuch horizental kuch vertical ho sakty perpendicular 


CSS units 
%
Percentage is that percent of his parent i.e if parent is body then that would be that percentage of body or else if a element has parent that has height 300px so inside element with 50% width will be 50% of parent that is 300px 
Vh and vw
Vh and vw are with reference with view port 
1vh is one percent of view port and view port jitna apky browser ki active window ya jinti jagah app chal rhi 
rem and em
Rem is relative to root font size i.e body 
It does not depend ap isko kisi b element ki class k andar use kro it always depends on root font size .. root ki css jo hm likhty 
Em is related to parent font size jitna parent class ka size hoga
pixel: it is absolute , doesn't depend on parent, so if we have a div of width 300px and total screen is 400px so onyl available space would be 300px so for reponsiveness, it will take the whole width and might go out of it as the width of mobile would be less than what we have given 





There are some properties that are inherited from parent to child but some are not 
If my parent have a class and that contain some propories or css so woh us k child par b apply hoti like color , line-height 
Can be seen here 
https://www.codecademy.com/resources/docs/css/inheritance






Important CSS Things

Line height : line height basically sets the height of a line and its inherited plus ek line mai if multiple div ya element tu jiski ziada hoti wohi usline ki height hoti..


Display properties
Block:: always start from new line and takes whole available space of the screen or depends on parent   . e.g p , div , h1 
We can set properties of height widht etc 
Inline::  start from where the space is available(cursor on the screen(where we are writing)) and takes the space its content depends on .. we cannot apply styles of widht height top etc on it  e.g. small , span , label 

Inline-block:: its like inline but we can appply styles of height width etc onit

Position Properties
Relative: apni jagah k hissab and create gap if moved
Absolute :  Always look for a parent with a position:relative , jdr b mily apny ancestors else body k hissab s . dont create gap on his side and element k oper neechy aa jata 
Static: static is default property , for Z-index the property should not be static .its like normal render flow  
Some Css properties
Top:  its like apny top eege s move kro itna distance, 
Bottom: its apny buttom s itna move kro 
Depends on postion attribute as well, incase of absolute look for parent , for relative apny s 




















Important tips:
Incase of positon absolute in a flex child , the flex properties dont work on it if top buttom etc is used, if used then look for relative parent .. if not used top bottom then align-slef b kam krta us p but space kha jata uski baqi bachy yani jab b ap absolute use krein gay woh apni jahah gap bna dy ga and baqi bachy woh jagah le sakty. But flex mai agr top-bottom krien gay tu woh flex s nikal jai ga 

