# CSS Simply Linear Preloader
This is a Simply Linear Preloader with or without logo / image / brand. Feel free to use this preloader in your project.

## Quick Start
HTML
```
<div class="fullscreen">
    <div class="preloader">
        <img src="assets/img/logo.png">
        <div class="bar-container">
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
    </div>
</div>
```
CSS
```
.fullscreen .preloader {
     position: fixed;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     z-index: 2000;
     background-color: #FFF;
     text-align: center;
     padding: 0;
}
 .fullscreen .preloader img {
     position: absolute;
     top: 40%;
     z-index: 2;
     margin: 0 auto;
     left: 0;
     right: 0;
     height: 50px;
}
 .fullscreen .preloader .bar-container {
     position: absolute;
     top: 50%;
     height: 4px;
     width: 130px;
     background-color: #eee;
     margin: 0 auto;
     left: 0;
     right: 0;
}
 .fullscreen .preloader .bar-container .bar {
     content: "";
     display: inline;
     position: absolute;
     height: 100%;
     width: 0;
     right: 0;
     background-color: #FFD32A;
}
 .fullscreen .preloader .bar-container .bar:nth-child(1) {
     animation: linear-animation 3s linear 1s infinite;
}
 .fullscreen .preloader .bar-container .bar:nth-child(2) {
     animation: linear-animation 3s linear 2s infinite;
}
 .fullscreen .preloader .bar-container .bar:nth-child(3) {
     animation: linear-animation 3s linear 3s infinite;
}
 @keyframes linear-animation {
     0% {
         right: 100%;
         width: 10%;
    }
     30% {
         right: 0%;
         width: 40%;
    }
     50% {
         right: 0%;
         width: 0%;
    }
     80% {
         right: 0%;
         width: 0%;
    }
     100% {
         right: 0%;
         width: 0%;
    }
}
```

JS (Required Jquery)
```
$(document).ready(function(){
    $('.fullscreen .preloader').fadeOut(5000);
});
```

## Ideas and Suggestions
Please kindly mail me at [teguh@circle-creative.com](mailto:teguh@circle-creative.com])
