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
