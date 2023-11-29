i just made some sass mixin for easier and faster coding... <br>
## Containing :
### 1.baseSetting : 
set base style setting ( font-family, font-size, text-color, link-color) <br>
### 2.icon and font : 
make pre made style for fonts and icons <br>
example : 
```
$fonts : (("name":normal,"size":16px,"weight":normal),
          ("name":bold,"size":16px,"weight":bold),
          ("name":"headline","size":20px,"weight":600));

@include font($fonts);
```
output :
```
.font-normal {
  font-size: 16px;
  font-weight: normal;
}

.font-bold {
  font-size: 16px;
  font-weight: bold;
}

.font-headline {
  font-size: 20px;
  font-weight: 600;
}
```
### 3.flex
contain display flex settings such as flex-direction, flex-wrap, justify-content,align-items

### 4.radius
border radius mixin for set all 4 radius in one line.
example :
```
@include radius((25px,65px,1px,0));
@include radius((25px,65px));
@include radius(20px);
```
output :
```
border-top-right-radius: 25px;
border-top-left-radius: 65px;
border-bottom-right-radius: 1px;
border-bottom-left-radius: 0;

border-top-right-radius: 25px;
border-top-left-radius: 25px;
border-bottom-right-radius: 65px;
border-bottom-left-radius: 65px;

border-radius: 20px;
```
### 5. card
card mixin with shadow and radius and padding
example :
```
@include card((20px,25px),5px,0 0 4px 0,red);
```
output :
```
.card {
  border-top-right-radius: 20px;
  border-top-left-radius: 20px;
  border-bottom-right-radius: 25px;
  border-bottom-left-radius: 25px;
  padding: 5px;
  box-shadow: 0 0 4px 0 red;
}
```
