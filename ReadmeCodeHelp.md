# Fonts and Colors

font-sizing --> Define Font ko kitna bada krna hai
font-weight -- Font ko kitna light ya bold krna hai
font-style -- font ka shada look krna hai italic me krana hai
font-family -- fonnt ka aapperance kaisa hona chahiye
line-height -- do line ke bich height dene ke liye
letter-spacing -- do letter ke bich space dene ke liye

# Colors
color : aqua
color : RGB(255 , 255 , 255 , opacity(0-1))
color : #RRGGBB (#FFFFFF)

# WE not apply height and width to span because it is inline element if you want to change there heght and width convert
display:inline-block;

# Box Model
AnyThing Render on Browser Always render on reactangular box no matter if it is cirle , spin , hollow but always apper in reactangular shape

Box-Model --> content , padding , border , margin

content --> jo bhi img , text wo mera condent

padding --> content ke aur border ke bich me jo gap hoga use hm padding bolte hai

border --> border to border hota hai

margin --> do box ke bich me jo gap hota hai use hm margin khte hai

margin : auto , hozontally bich me laa deta hai

# Box-sizing:border-box rkhna ek good practise kyu hai ?
Kyuki border-box rkhne se hme jitna width aur height ka box chihiye utna mila jata hai.

suppose muzhe 200*200 ka box chahiye , content ka size hamara 200 * 200 hai padding 10px ki hai aur border 5px ki hai

to hamara box 200 * 200 hoga jisme border + padding + content ko milake width 200 and height 200 hongi

if border-box nhi dete to box-size bd jata hai

# What is Display
Hme apne tag ko kis tarh se dikhana hai display kran hai use hm display bolte hai (div , a, img)

Display : inline , Block , inline-block , none

Block :- By default take full width
        start With New Line
        width/height -- applicable
        margin/padding -- applicable

Inline : - By defult take content hi width
           start with same line if width remain
           width/height --> not applicable
           margin --> horizontal applicable , vertically not applicable
           padding --> applicable

Inline-Block : Behave as Inline 
               but custome width/height/margin/padding - applicable

# Position --> mere pass bhut se tag hai unhe muzhe position krna hai apne page me kis kis trh se position krna hai use position me add krna hai , by default position static hota hai

position --> static , relative , absolute , fixed

Postion : By default Static --> Jisme na app top , left , right , bottom , z-index koi property apply nhi kr skte

relative : relative to itselef and current window 
  using left , top , right , bottom --> spacing define
  position ki gap retained rhti hai

absolute > absolute to its closest positioned ancestor

  using left , top , right , bottom --> spacing define

  gap retained nhi rthi uski gap me usse just next box palced ho jata hai

  absoute krne se ye box one layer upper jati hai

fixed :- fixed that postion in full window
 
     using left , right , top , bottom --> spacing define

     gap retained nhi rhti us gap me usse just next wala box placed ho jata hai

     fixed krne se one layer upper aa jati hai but fixed rhti hai pure window me

sticky : sticky deke use top , left , bottom , right , position delhe use ek jagh stcky kra do
  
 then wo fixed rhti hai apne parent container me , jaise hi parent container se bahar aati hai wo static ho jati hai

# ABSOLUTE AND RELATIVE UNIT

RELATIVE --> (Relative means relative to someone , may by window , may be parent) vh , vw , % , rem , em
ABSOLUTE ---> Absolute hamesha absolute hi rhega 25px

Percentage (%) Relative to there parent

        .web{
            border: 1px solid gold;
            background-color: tomato;
            color: white;
            /* 50% to there parent , in this case there parent is body so it take 50% of body */
            width: 50%;
        }
        .parent{
            border: 1px solid red;
            background-color: wheat;
        }
        .child{
            border: 1px solid green;
            background-color: yellow;
            /* width 50% of parent div */
            width: 50%;
        }

<div class="web">
        Welcome To Web-Development
    </div>
    <div class="parent">
        <div class="child">child Box</div>
</div>

VH and VW --> Relative to ViewPort Height or Width (max (0-100)vh or (0-100)vh)

<div style="width:50vh; height 50vh">
     Welcome To My Journey
</div>


Pixel --> 1px -> 1/96 * inch

# Homework what is physical and logical pixel
# Homework ppi and dpi difference

em --> Relative to parent (ont size of the parent, in the case of typographical properties like font-size, and font size of the element itself, in the case of other properties like width)

by default font-size is 16 px

.chid{
    font-size : 10em (10 * 16 ==> 160px)
}

suppose

.parent{
    font-size : 5px
}

.child{
    font-size : 10em (10*5) --> 50px
}

<div class="parent">
        <div class="child">
            Child 1
        </div>
</div>

# Use Relative uniti to make our website Responsive

rem --> Relative to root element  root element in html is html tag(Font size of the root element.)

by default root element font-size ==> 16px

.parent{
    font-sizing : 10rem(10*16px ==> 160px)
}


Float VS Clear 

Overflow : visible by default 
        : hidden (jitna bhi text overflow ho rha use delete krta hai)
        :scroll (ek scroll bnata jisse overflow hone wala dekh skte hai)
        : auto (apne hisab se scroll add krta hai horizontal vertical)

Float : Basically box ko layout ke liye use krte hai but abhi modern smy me flex ka use kiya jata hai

Float ka use normal use ke liye ka jata hai jaise ki img aur paragraph ek saat dikhana hai jaise ki wikipidia me dikhta hai