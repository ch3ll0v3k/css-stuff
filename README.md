#####handy-dandy CSS snippet

#####Info
```javascript

["http://www.mydevice.io/"]

[4:3 'aspect ratio resolutions']:
    640×480, 800×600, 960×720, 1024×768, 1280×960, 1400×1050, 
    1440×1080, 1600×1200, 1856×1392, 1920×1440, 2048×1536

[16:10 'aspect ratio resolutions']:
    1280×800, 1440×900, 1680×1050, 1920×1200, 2560×1600

[16:9 'aspect ratio resolutions']:
    1024×576, 1152×648, 1280×720, 1366×768, 1600×900, 1920×1080, 2560×1440, 3840×2160


[ 23.2% - 1366 x 768  ]
[ 20.2% - ** OTHER ** ]
[ 14.5% - 1920 x 1080 ]
[ 13.4% - 768  x 1024 ]
[ 7.6%  - 1028 x 800  ]
[ 6.3%  - 1440 x 900  ]
[ 3.6%  - 1600 x 900  ]
[ 3.2%  - 1024 x 768  ]
[ 2.7%  - 1680 x 1050 ]
[ 1.7%  - 2560 x 1440 ]
```

#####CSS [0]:
```css
/* <= 360px */
@media only screen and (max-width: 360px){}
@media only screen and (max-width: 360px) and (orientation : landscape){}
@media only screen and (max-width: 360px) and (orientation : portrait){}

/* 361px - 480px */
@media only screen and (min-width: 361px) and (max-width: 480px) {}
@media only screen and (min-width: 361px) and (max-width: 480px) and (orientation : landscape){}
@media only screen and (min-width: 361px) and (max-width: 480px) and (orientation : portrait){}

/* 481px - 640px */
@media only screen and (min-width: 481px) and (max-width: 640px) {}
@media only screen and (min-width: 481px) and (max-width: 640px) and (orientation : landscape){}
@media only screen and (min-width: 481px) and (max-width: 640px) and (orientation : portrait){}

/* 641px - 768px */ /* [ 13.4% - 768  x 1024 ] */
@media only screen and (min-width: 641px) and (max-width: 768px) {}
@media only screen and (min-width: 641px) and (max-width: 768px) and (orientation : landscape){}
@media only screen and (min-width: 641px) and (max-width: 768px) and (orientation : portrait){}

/* 769px - 1024px */ /* [ 3.2%  - 1024 x 768  ] */
@media only screen and (min-width: 769px) and (max-width: 1024px) {}
@media only screen and (min-width: 769px) and (max-width: 1024px) and (orientation : landscape){}
@media only screen and (min-width: 769px) and (max-width: 1024px) and (orientation : portrait){}

/* 1025px - 1280px */
@media only screen and (min-width: 1025px) and (max-width: 1280px) {}
@media only screen and (min-width: 1025px) and (max-width: 1280px) and (orientation : landscape){}
@media only screen and (min-width: 1025px) and (max-width: 1280px) and (orientation : portrait){}

/* 1281px - 1440px */ /* [ 23.2% - 1366 x 768  ] */ /* [ 6.3%  - 1440 x 900  ] */
@media only screen and (min-width: 1281px) and (max-width: 1440px) {}
@media only screen and (min-width: 1281px) and (max-width: 1440px) and (orientation : landscape){}
@media only screen and (min-width: 1281px) and (max-width: 1440px) and (orientation : portrait){}

/* 1441px - 1680px */ /* [ 3.6%  - 1600 x 900  ] */ /* [ 2.7%  - 1680 x 1050 ] */
@media only screen and (min-width: 1441px) and (max-width: 1680px) {}
@media only screen and (min-width: 1441px) and (max-width: 1680px) and (orientation : landscape){}
@media only screen and (min-width: 1441px) and (max-width: 1680px) and (orientation : portrait){}

/* 1681px - 1920px */ /* [ 14.5% - 1920 x 1080 ] */
@media only screen and (min-width: 1681px) and (max-width: 1920px) {}
@media only screen and (min-width: 1681px) and (max-width: 1920px) and (orientation : landscape){}
@media only screen and (min-width: 1681px) and (max-width: 1920px) and (orientation : portrait){}

/* 1921px - 2560px */ /* [ 1.7%  - 2560 x 1440 ] */
@media only screen and (min-width: 1921px) and (max-width: 2560px) {}
@media only screen and (min-width: 1921px) and (max-width: 2560px) and (orientation : landscape){}
@media only screen and (min-width: 1921px) and (max-width: 2560px) and (orientation : portrait){}

/* 2561px >> */ /* 4k - 8k - 16k ?? */
@media only screen and (min-width: 2561px) {}
@media only screen and (min-width: 2561px) and (orientation : landscape){}
@media only screen and (min-width: 2561px) and (orientation : portrait){}

```

#####CSS [1]:
```css

@media not|only mediatype and (media feature) {
    // ...
}

@media only screen 

    and (min-width: 481px)
    and (max-width: 640px)
    and (orientation : landscape)
    
    and (min-color-index: 256)
    
    and (min-aspect-ratio: 1/1)
    and (device-aspect-ratio: 16/9)
    and (device-aspect-ratio: 16/10)

    and ( -webkit-min-device-pixel-ratio: 1.5)
    and ( -moz-min-device-pixel-ratio: 1.5)
    and ( -o-min-device-pixel-ratio: 1.5)
    and ( min-device-pixel-ratio: 1.5)

    and ( -webkit-device-pixel-ratio: 3/2 )
    and ( -moz-device-pixel-ratio: 3/2 )
    and ( -o-device-pixel-ratio: 3/2 )
    and ( device-pixel-ratio: 3/2 )


{

    // ...
    // ...
    // ...

}

```


#####HTML [0]:
```html

<link rel="stylesheet" media="all and (min-color-index: 256)" href="stl.css" />
<link rel="stylesheet" media="media screen and (min-aspect-ratio: 1/1)" href="stl.css" />
<link rel="stylesheet" media="media screen and (device-aspect-ratio: 16/9), screen and (device-aspect-ratio: 16/10)" href=""/>

```

#####Media Types:
```
<link rel="stylesheet" media="mediatype and|not|only (media feature)" href="stl.css">

Value                   : Description
----------------------- : ----------- 
all                     : Used for all media type devices
aural                   : Deprecated. Used for speech and sound synthesizers
braille                 : Deprecated. Used for braille tactile feedback devices
embossed                : Deprecated. Used for paged braille printers
handheld                : Deprecated. Used for small or handheld devices
print                   : Used for printers
projection              : Deprecated. Used for projected presentations, like slides
screen                  : Used for computer screens, tablets, smart-phones etc.
speech                  : Used for screenreaders that "reads" the page out loud
tty                     : Deprecated. Used for media using a fixed-pitch character grid, like teletypes and terminals
tv                      : Deprecated. Used for television-type devices

```

####Media Features:
```
Value                   : Description
----------------------- : ----------- 
aspect-ratio            : The ratio between the width and the height of the viewport
color                   : The number of bits per color component for the output device
color-index             : The number of colors the device can display
device-aspect-ratio     : The ratio between the width and the height of the device
device-height           : The height of the device, such as a computer screen
device-width            : The width of the device, such as a computer screen
grid                    : Whether the device is a grid or bitmap
height                  : The viewport height
max-aspect-ratio        : The maximum ratio between the width and the height of the display area
max-color               : The maximum number of bits per color component for the output device
max-color-index         : The maximum number of colors the device can display
max-device-aspect-ratio : The maximum ratio between the width and the height of the device
max-device-height       : The maximum height of the device, such as a computer screen
max-device-width        : The maximum width of the device, such as a computer screen
max-height              : The maximum height of the display area, such as a browser window
max-monochrome          : The maximum number of bits per "color" on a monochrome (greyscale) device
max-resolution          : The maximum resolution of the device, using dpi or dpcm
max-width               : The maximum width of the display area, such as a browser window
min-aspect-ratio        : The minimum ratio between the width and the height of the display area
min-color               : The minimum number of bits per color component for the output device
min-color-index         : The minimum number of colors the device can display
min-device-aspect-ratio : The minimum ratio between the width and the height of the device
min-device-width        : The minimum width of the device, such as a computer screen
min-device-height       : The minimum height of the device, such as a computer screen
min-height              : The minimum height of the display area, such as a browser window
min-monochrome          : The minimum number of bits per "color" on a monochrome (greyscale) device
min-resolution          : The minimum resolution of the device, using dpi or dpcm
min-width               : The minimum width of the display area, such as a browser window
monochrome              : The number of bits per "color" on a monochrome (greyscale) device
orientation             : The orientation of the viewport (landscape or portrait mode)
overflow-block          : How does the output device handle content that overflows the viewport along the block axis (added in Media Queries Level 4)
overflow-inline         : Can content that overflows the viewport along the inline axis be scrolled (added in Media Queries Level 4)
resolution              : The resolution of the output device, using dpi or dpcm
scan                    : The scanning process of the output device
update-frequency        : How quickly can the output device modify the appearance of the content (added in Media Queries Level 4)
width                   : The viewport width
```
