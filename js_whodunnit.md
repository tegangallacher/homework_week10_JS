JS Day 1 Homework

Go through each sample code and work out what the output will be and explain what happened.

Episode 1

var name = 'Keith';

var printName = function() {
  console.log('My name is ' + name );
};

printName();
****Answer Episode 1 = My name is Keith


Episode 2

score = 5;

var result = function() {
  var score = 3;
  return score;
};

console.log(result());
****Answer Episode 2 = 3

Episode 3

var myAnimals = ['Chickens', 'Cats', 'Rabbits'];

var listAnimals = function() {
  myAnimals = ['Ducks', 'Dogs', 'Lions'];
  for(var i=0;i<myAnimals.length; i++){
    console.log(i + ": " + myAnimals[i]);
  }
}

listAnimals();
****Answer Episode 3 = 
0: Ducks 
1: Dogs 
2: Lions

Episode 4

var suspectOne = 'Jay';
var suspectTwo = 'Val';
var suspectThree = 'Keith';
var suspectFour = 'Rick';

var allSuspects = function() {
  var suspectThree = 'Harvey'
  console.log('Suspects include: ' + suspectOne + ', ' + suspectTwo + ', ' + suspectThree + ', ' + suspectFour)
};

allSuspects();
console.log( 'Suspect three is:' + suspectThree );
****Answer Episode 4 = "Suspcts include: Jay, Val, Harvey, Rick" & "Suspect three is: Keith"

Episode 5

var detective = {
  name : 'Ace Ventura',
  pet : 'monkey'
};

var printName = function(detective) {
  return detective.name
};

var detectiveInfo = function() {
  detective['name'] = 'Poirot'
  return printName(detective);
};

console.log(detectiveInfo());
****Answer Episode 5 = Poirot

Episode 6

var murderer = 'rick';

var outerFunction = function() {
  var murderer = 'marc';

  var innerFunction = function() {
    murderer = 'valerie';
  }

  innerFunction();
}

outerFunction();
console.log('the murderer is ', murderer);
****Answer Episode 6 = the murder is rick


Episode 7 - Make up your own episode/s!

Make up your own episode which can be whatever you wish and the rest of the class will work out together what happened and what the output will be.

var victim = {
  name : 'Lewis',
  death : 'stabbing'
};

var printDeath = function(victim) {
  return victim.death
};

var victimInfo = function() {
  victim['death'] = 'poison'
  return printDeath(victim);
};

console.log(victim.name, ": death by", victimInfo());