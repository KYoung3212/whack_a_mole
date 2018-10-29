# Whack-A-Mole Game
The Whack-A-Mole interactive game for mobile/desktop displays my ability to be able to create a React JS application from scratch.  Making sure to focus on a modern, sleek, and user-friendly experience, my Whack-A-Mole game gives the user a smooth, yet challenging experience.

Built in React.<br>
Animation with [Anime.js](http://anime-js.com/).<br>
Illustration designed in Adobe Illustrator.<br>
Created with the [create-react-app](https://www.npmjs.com/package/create-react-app) npm module. <br>
Hosted on Heroku.<br>

You can test it on my [live demo].

<img src="https://github.com/KYoung3212/whack_a_mole_react/blob/master/public/assets/illustration-for-readme.gif" width="320">

## Screenshots
<img src="https://github.com/KYoung3212/portfolio/blob/master/img/slides/whack-0.jpg" width="320">
<img src="https://github.com/KYoung3212/portfolio/blob/master/img/slides/whack-1.jpg" width="320">
<img src="https://github.com/KYoung3212/portfolio/blob/master/img/slides/whack-2.jpg" width="320">


## Features

  - A modern/user-friendly mobile/desktop game built entirely in React JS.
  - Responsive design allows for ease of usage from both desktop and mobile access.

## Planned Features
  - Integrate a leaderboard to display the highest number of scores of the day/month
  - Integrate a login feature for the user to keep track of their score history.
  - Set up a MySql database to keep track of user scores, leaderboards, and date/times.

## Personal Insight
> The Whack-A-Mobile App  is a personal achievement of mine because I was able to create a fun, yet challenging experience for the user.  This project improved my React JS skills significantly, working out errors and bugs which would not have been present in Javascript.

> After fully implementing all front-end features, I made a few changes to make the user experience a smoother. 

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


## Contributions
I have always been a person to continutally want to improve any of my projects since there is always room for improvement.  If you would like to contribute please reach out via [email]: kevin.young3212@yahoo.com or you can reach me directly at my [portfolio]. Thanks!

   [live demo]: <http://whack-a-mole.kevin-young.us>
   [email]: <http://kevin.young3212@gmail.com>
   [portfolio]: <https://kevin-young.us>



