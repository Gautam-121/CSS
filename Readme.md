# Level-1

importance -> Inline > internal and external 

internal and external me importance jo niche likha ho wo apply hota hai

# Level-2

background-color => background ke phichr lgta hai
color : RGB(255 , 255 , 255) , RGBA(255 , 255 , 255 , opacity control) HEX(#RRGGBB)

opacity contaol (0 to 1) 0 -> Totally Transperant , 1 -> Fully Visible

bacground-image -> learn more and visibillity -> learn more

background-color : red (its set the backhead colour of box)
background-image : url(path) (its set the background imgage)

if -> Your box width is 50px and height is 50px and you want to image contain
your box size 

contain
Scales the image as large as possible within its container without cropping or stretching the image. If the container is larger than the image, this will result in image tiling, unless the background-repeat property is set to no-repeat.
use ==> background-size :  contain 
        background-repeat : no-repeat (if contain img full img space is free it start repeat the img but you don't wnat to reapeat set no-repeat)
  
cover -> it will streach the img and cover full height and width by cropping the img
Scales the image (while preserving its ratio) to the smallest possible size to fill the container (that is: both its height and width completely cover the container), leaving no empty space. If the proportions of the background differ from the element, the image is cropped either vertically or horizontally.
  backgound-size : cover

background-attachment:scroll ,fixed , local

body kr liye background image scroll hoti hai --> scroll yani text down scroll krne pr
image bhi down scroll hongi , if fixed krna hai background-image ko to fixed property use krna pdta hai , yha local se kuch fark nhi pdta hai

div -> contain ke liye background-image by defauld fixed hoti hai  --> fixed yani scroll krne pr imgage whi rhengi --> if imgae bhi scroll ho wo krna hai to yha local ka use krna pdege --> scroll se kuch fark nhi pdta yha


visibillity --> property jisse box to wha rhega wo height bhi lenga width bhi lenga jitna diya ho pr visible nhi haonga if hidden kra ho


# Text-Align Property

we only control horizontal alignment of text within a box

values -> can take left , center , right

# Text-decoration Property

modified the apperance of inline text
Options include none , underline , overline , line-throught
hyperlinks - commanly used to remove underlines from hyperlinks

values -> underlines , dashed , double , solid , wavy

# Text-transform

values => uppercase , lowercase , capitalize , none

# line-height
Adjust the amount of space above and below in inline element

# font-size
Sets the size of font in web content

# font-weight
Defines the thickness of characters in a font

# font-style
italic , oblique , normal

# font-family
add font family of 

# Level-5

# Display Property
Block Element --> it take full screen of width and start with next line

Inline Element --> It take content width and it start from same line (but ou cant set heighr and width easily)

Inline-Block --> inline-block kya bolta hai , muzhe block ki property bhi apne hisib set set krna hai to app dikhao inline hi lekin mai block ke property bhi change kr skta hu

display:none --> if ui se koi box delete ho gya mtlab wo gayab ho gya but abhibhi wo size le rha hai to display:none krne se wo suze bhi nhi lega 

# Relative Units

(Percentage) --> Facinatting Dynamic Sizing Relative to there Parents , if there is no parent then it take it body as parent

(EM)--> Sized Relative to the parent element's font size

Font-Sizing : Commanly Used For Setting Font Sizes Adaptively

(REM)--> Facilatting Dynamic sizing relative to root element (root in basically in our case body)


VW/VH --> mere screen me jo view display ho rha hai wo mera width mera khlata hai view width(vw) and view height khlata hai (view height)

kisibhi cheez ki size hme sirf parent se nhi pure viewport se define krni hai

100vh --> 100% of viewport height
100vw --> 100% of viewport width


# Position Property

Position By Default (Static) : Element follow the normal document flow (top , right , bottom , left , z-index would not work)

static me box page ke saat chipka rhta hai

Position : Relative :- Relative to itself (right : 10px) to khudki actual postion jo thi uski relative me right : 10px ho gya

Relative me bhi box page ke saat chipka rhta hai

Position : Absolute :- Absolute apni position dekhta hi nhi wo hmesha page ke corner se start hota hai

right : 50px
bottom : 50px  50px 50px move krega from page ka coner , parent se mtlab nhi , khud se mtlab nhi , corner se wo moved kr dega

Absolute dete hi wo page root uper aa jata hai yani page se bahar aa jata hai aur uski jagah usse niche wala box le leta hai

ye page se bahar hone ke wajah se page ke under jo rhenge uspe chadte dikhenge

Position : Fixed 
Fixed as same as absolute lekin isme scroll hai wo bhi nhi chalata 
yani ye page se bahar ho jata hai phir page ka contain uper niche kro ye whi fixed rhta hai
navigation serach bar me ye use krte hai

all same as absolute only diffrent ye page ke saat scroll nhi hoga apni position me hi rhega

learn About Z-index
