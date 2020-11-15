# genbuildings

A Clojure library designed to generate genetic buildings within the context of [The Great Game](https://simon-brooke.github.io/the-great-game/) framework, implementing and developing ideas described in [Modelling rural to urban, take two](https://blog.journeyman.cc/2013/10/modelling-rural-to-urban-take-two.html).

## Usage

Broadly, for a type of building, a build function will be a function which takes as arguments

1. A `vertex`, being a two dimensional point where each dimension is an integer in the range 0...1x10^9, considered as a number of millimetres;
2. A `heading`, being a real number in the range 0...360 (or possibly we may use radians, if that turns out to be simpler;
3. A `world`, being a data structure as described in [the-great-game.world.world](https://simon-brooke.github.io/the-great-game/codox/the-great-game.world.world.html);
4. A `culture`, being a keyword identifying a culture within that world;
5. A `holder`, being a data structure as described in [the-great-game.agent.agent](https://simon-brooke.github.io/the-great-game/codox/the-great-game.agent.agent.html);
6. `units`, being an integer in the range 1...100 (but for normal buildings more typically 1...10) defining the number of building units (roughly, rooms) in the building.

and returning a renderable model of a building, such that in a large game world identical building models will be generated rarely.

## Copyright and Licence

Copyright © 2020 Simon Brooke; licenced under the
[GNU General Public Licence](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html), either version 2 or, at your option, any later version.

