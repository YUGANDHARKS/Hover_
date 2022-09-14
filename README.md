# Hover_
#Hover Function
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Hover Me</title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <style type="text/css">
            *{
                padding: 0;
                margin: 0;
                box-sizing: border-box;
                font-family: "Poppins",sans-serif;
            }
            body {
                background-color: #f0f5ff;
            }
            p{
                width: 100%;
                position:absolute;
                transform: translate(-50%,-50%);
                left: 50%;
                top: 50%;
                background-color: white;
                padding: 3.5em;
                text-align: center;
                font-size: 16px;
            }
            a{
                position: relative;
                color: orange;
                font-size: inherit;

            }
            a:after{
                position: absolute;
                width: 12em;
                background-color: #202842;
                content: attr(data-tip);
                padding: 0.6em 0;
                color: #ffffff;
                margin: auto;
                left: -4.5em;
                right: 0;
                bottom: 1.5em;
                text-align: center;
                border-radius: 0.2em;

            }
            a:before{
                position: absolute;
                content: "";
                height: 0;
                width: 0;
                border-top: 0.5em solid #202842;
                border-left: 0.5em solid transparent;
                border-right: 0.5em solid transparent;
                margin: auto;
                left: 0;
                right: 0;
                bottom: 1em;

            }
            a:before,
            a:after{
                display: none;
            }
            a:hover:before,
            a:hover:after{
                display: block;
            }
        </style>
    </head>
    <body>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi, odio commodi?<a href="#" data-tip="Welcome">Designteam</a>
             Error earum debitis enim alias dolore. <a href="#" data-tip="Thank you">LX Design</a>    Possimus, deleniti incidunt eum
              commodi nostrum ducimus placeat, sit fuga esse illum molestiae.
        </p>
    </body>
</html>
