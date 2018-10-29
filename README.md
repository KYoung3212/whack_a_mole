# Whack-A-Mole Game
The Airbnb Website Template for the mobile application displays my ability to be able to create a website for a product from scratch.  Making sure to focus on a modern, sleek, and user-friendly experience, the Airbnb Website tries to grab the users attention to download the mobile application.

You can test it on my [live demo].(https://kevin-young.us/whack_a_mole).

<img src="https://github.com/KYoung3212/whack_a_mole_react/blob/master/public/assets/illustration-for-readme.gif" width="320">

Built in React.<br>
Animation with [Anime.js](http://anime-js.com/).<br>
Illustration designed in Adobe Illustrator.<br>
Created with the [create-react-app](https://www.npmjs.com/package/create-react-app) npm module. <br>
Hosted on Heroku.<br>

The Airbnb Website Template for the mobile application displays my ability to be able to create a website for a product from scratch.  Making sure to focus on a modern, sleek, and user-friendly experience, the Airbnb Website tries to grab the users attention to download the mobile application.

You can test it on my [live demo]. 

## Screenshots
<img src="https://github.com/KYoung3212/portfolio/blob/master/img/slides/airbnb-0.jpg" width="320">
<img src="https://github.com/KYoung3212/portfolio/blob/master/img/slides/airbnb-1.jpg" width="320">
<img src="https://github.com/KYoung3212/portfolio/blob/master/img/slides/airbnb-2.jpg" width="320">


## Features

  - A modern/user-friendly front-end site displaying the new Airbnb Mobile Application.
  - Responsive design allows for ease of usage from both desktop and mobile access.
  - Responsive Slick Carousel, showing the mobile application screenshots to the user.
  - Video access of the application to show the user a hands-on walkthrough of the application.
  - Contact form with PHP/Backend setup for the user to easily contact the company with any questions.

## Planned Features
  - Integrate Javascript to allow the user to click on the routing links to be able to fully download the application.
  - Customizable theme options for the user to choose from based on their preferred style.
  - Condensing load times of the web page, improving infinite scroll, image sizing, and pre-load. 

## Personal Insight
> The Airbnb Mobile App Template is a personal achievement of mine because I was able to build the front-end site of a product to grab the eye of the user. Making sure to keep everything looking modern, I was able to create a site that could potentially pass as an official Airbnb Website.  

> After fully implementing all front-end features, I made a few changes to make the user experience a bit smoother, for example with load times. 


## Contributions
I have always been a person to continutally want to improve any of my projects since there is always room for improvement.  If you would like to contribute please reach out via [email]: kevin.young3212@yahoo.com or you can reach me directly at my [portfolio]. Thanks!

   [live demo]: <https://kevin-young.us/whack_a_mole)>
   [email]: <http://kevin.young3212@gmail.com>
   [portfolio]: <https://kevin-young.us>



### Key learnings:

Calling functions in a component from a different component by passing onClick() in the props:<br>

#### App.js:<br>
The timeOut function is defined in App.js.
```
<StartButton context={ this.state } onClick={ this.timeOut.bind(this) }/>
```

#### StartButton.js:<br>
The timeOut function in App.js is called via the onClick on the component in StartButton.js
```
render(){
  return (
    <button className="game__start-button" type="button"
      onClick={ this.props.onClick } style={{ display: this.props.context.buttonDisplay }}>
      { this.props.context.buttonMessage }
    </button>
  )
};
```
