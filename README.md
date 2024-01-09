<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="newcard.css">
    <title>Animated Flex Cards</title>
    <style>
        * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
}

body {
    background-color: #eeeeea;
}

.wrapper {
    width: 100%;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.container {
    height: 400px;
    display:flex;
    flex-wrap:auto;
    justify-content: start;
}

.card {
    width: 88px;
    border-radius: .76rem;
    background-size: cover;
    cursor: pointer;
    overflow: hidden;
    border-radius: 2rem;
    margin: 0 10px;
    display: flex;
    align-items: flex-end;
    transition: .6s cubic-bezier(.28,-0.03,0,.99);
    box-shadow: 0px 10px 30px -5px rgba(0,0,0,0.8);
}

.card > .row {
    color: white;
    display: flex;
    flex-wrap: nowrap;
}

.card > .row > .icon {
    background: #223;
    color: white;
    border-radius: 50%;
    width: 55px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 15px;
}

.card > .row > .description {
    display: flex;
    justify-content: center;
    flex-direction: column;
    overflow: hidden;
    height: 74px;
    width: 525px;
    opacity: 0;
    transform: translateY(40px);
    transition-delay: .3s;
    transition: all .3s ease;
}

.description p {
    color: #b0b0ba;
    padding-top: 5px;
}

.description h4 {
    text-transform: uppercase;
}

input {
    display: none;
}

input:checked + label {
    width: 600px;
}

input:checked + label .description {
    opacity: 1 !important;
    transform: translateY(0) !important;
}

.card[for="c1"] {
    background-image: url('https://img.freepik.com/premium-photo/3d-render-boy-character-with-glasses-generative-ai_384720-2045.jpg');
}
.card[for="c2"] {
    background-image: url('https://i.pinimg.com/474x/55/07/52/550752eb5dc9b567536001e547bea757.jpg');
}
.card[for="c3"] {
    background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTgxcpIlaOXfFE4dof91-omf899xzzUcPC1qbqWDSDAKwUe0bU6XkNf1QzJThunQc5ypYE&usqp=CAU');
}
.card[for="c4"] {
    background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTGbsCBagPMn1iho94G_PmHxLS70PFZLGCvfMaBVOJ-nTPeLbdhSflvvGC0I0Ss2ryiyjo&usqp=CAU');
}
    </style>
</head>
<body>
    <div class="wrapper">
        <div class="container">
            <input type="radio" name="slide" id="c1" checked>
            <label for="c1" class="card">
                <div class="row">
                    <div class="icon">1</div>
                    <div class="description">
                        <h4>Winter</h4>
                        <p>Winter has so much to offer -
                         creative activities</p>
                    </div>
                </div>
            </label>
            <input type="radio" name="slide" id="c2" >
            <label for="c2" class="card">
                <div class="row">
                    <div class="icon">2</div>
                    <div class="description">
                        <h4>Digital Technology</h4>
                        <p>Gets better every day -
                         stay tuned</p>
                    </div>
                </div>
            </label>
            <input type="radio" name="slide" id="c3" >
            <label for="c3" class="card">
                <div class="row">
                    <div class="icon">3</div>
                    <div class="description">
                        <h4>Globalization</h4>
                        <p>Help people all over the world</p>
                    </div>
                </div>
            </label>
            <input type="radio" name="slide" id="c4" >
            <label for="c4" class="card">
                <div class="row">
                    <div class="icon">4</div>
                    <div class="description">
                        <h4>New technologies</h4>
                        <p>Space engineering becomes
                         more and more advanced</p>
                    </div>
                </div>
            </label>
        </div>
    </div>
</body>
</html>
