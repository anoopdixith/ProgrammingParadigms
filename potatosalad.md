With *"Functional Programming"*, from being regarded as the paradigm of "academia and research", finally making its presence evident in commercial and enterprise applications, I thought it's worth understanding the difference between three major programming paradigms in use today. And after this Potato Salad Kickstarter campaign, I realize there's no better way to do this than via preparing potato salad.

**1. Imperative Programming:**   
This is a style of programming where the state of the program changes due to execution of statements. Procedural programming is a part of this wherein "procedures"/"functions"/"subroutines" bundle the statements. E.g. C Programming language. 

So, let's prepare the salad the 'imperative way'.

        imperative_potato_salad(pepper,salt) {
                potatoes = bring_potatoes();
                tender_cook_in_boiling_water(potatoes); 
                combine_and_mix(potatoes, pepper, salt);
        }

As we can see, the whole thing at the end boils down to execution of statements that change the state of datafields.

**2. Functional Programming:**
This style of programming avoids mutation and program states by mostly treating computations as evaluating mathematical expressions. Unlike imperative programming model, this doesn't explicitly state the intermediate steps of achieving something. One of the significant features of most Functional Programming languages is that they treat functions/subroutines as "first-class-entities", meaning you can actually pass functions as arguments (damn, how I wish Java allowed this). 
While Haskell is referred as a "Pure Functional Programming Language" (Qualifier 'pure' indicates no operation has 'side effects' and 'side effect' means that evaluating a particular expression changes some internal state of the system because of which, evaluation of the same expression later would give a different result), another biggie in this area, "Erlang", is an impure functional programing language. Well, due to the increasing demand for concurrent services, Erlang now forms the backbone of some of the widely used massive client-base services like Facebook Chat, messenger giant Whatsapp, CouchDB, queuing mogul RabbitMQ, (a part of) GitHUB and many more. The point I'm trying to make is that irrespective of whether you're an imperative person or a functional dude or an oops fan, it's good for you to know to code in Erlang.  So let's make potato salad in Erlang.

        -module(potato_salad).
        -export([prepare/3]).
        prepare(potatoes, salt, pepper) -> mix_well(boil(potatoes), salt, pepper).

Notice the use of first-class functions.

**3. Object Oriented Programming:**
Aah, here it cometh. Paradigm where "object"s, the instances of "class"es, have datafields (what they have) and methods/procedures (what they can do). While some languages like Ruby and Scala are called purely OOP languages in a sense that everything from characters to modules are treated as objects, most OOP languages are not pure. For e.g. Java isn't (remember 'int', 'Integer' and autoboxing stuff?). OOP was primarily intended at increasing reusability and modularity. However, it has been consistently criticized for failing to efficiently achieve the same stated goals. Developer of Erlang, Joe Armstrong once said "The problem with object-oriented languages is they've got all this implicit environment that they carry around with them. You wanted a banana but what you got was a gorilla holding the banana and the entire jungle."
Anyway, let's make our final version of goddamn potato salad.

        public class PotatoSalad  {
                 private Potato potato;
                 private Salt salt;
                 private Pepper pepper;
                
                 public PotatoSalad(Potato potato, Salt salt, Pepper pepper) {
                         this.potato = potato;
                         this.salt = salt;
                         this.pepper = pepper;
                 } 
        
                public void boilAndMix(Potato potato, Salt salt, Pepper pepper) {
                /* Well, boil and mix. We don't have APIs for them yet. Hey, startup idea. Develop a digital interface for a stove. The interface receives POST  requests to lightTheStove, stir, turnOff and GET requests to checkFoodStatus. And then release an SDK to let developers write apps leveraging the power of these APIs. The apps must allow users to share what they're cooking and let their friends rate it, on Facebook - "Preparing potato salad. I rated myself 5 out of 5 in making salads. -- updated via SmartCook app. */ 
                }
        }

Well, there are many other programming paradigms like event-driven programming (E.g. ActionScript) , Aspect Oriented Programming (AOP) etc which are worth looking into. However, I'm gonna stop here because I'm hungry and wanna eat the 3 kinds of salad I just prepared.
