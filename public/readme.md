#Emigma X
---
coded by Tobias Toland <br>
version 1.062 <br>
encryption engine ♞♞ 


Enigma X is based on the <a href="https://en.wikipedia.org/wiki/Enigma_machine">German WWII code machine</a>. Since coding Enigma simulators is popular I wanted to do something unique. This is my attempt to make a more secure Enigma using the basic components of the original machine. It was also my very first JavaScript, and CSS project.

Enigma X will take any basic <a href="https://en.wikipedia.org/wiki/ASCII">ASCII</a> message and encrypt it to "Think Ding", a special character set made of 26 Unicode symbols. To do this it translates each ASCII character into two Enigma characters (a letter from A-Z) and then pushes them through a randomly configured <a href="https://en.wikipedia.org/wiki/Enigma_machine#Plugboard">plugboard</a> and 26 randomly selected and configured <a href="https://en.wikipedia.org/wiki/Enigma_rotor_details">Enigma rotors</a>. Each message also has an added random key encoded within itself that is used to send the message again through a second set of 3 rotors so no two encodings will be the same. Finally the message is encoded to "Think Ding".

My basic security ideas are 1. Remove the <a href="https://en.wikipedia.org/wiki/Enigma_machine#Reflector">reflector</a> so any letter can be encoded to itself 2. Increase the size of the key by a bunch (that's a technical term) 3. Add random variability to every message encoded.

I have attempted to make Enigma X as secure as possible. In the end I am at best an amatuer crypographer and this is based on a machine notorious for being broken before the age of computers. It is safe to say this encryption scheme is dubious. With that said, Enigma X is just for fun and education. If anyone has any good ideas for breaking it I'd love to hear about them.

Enigma X is pure JavaScript, HTML, and CSS, with direct DOM manipulation. It does not use JQuery! The only thing not hand crafted by myself is <a href="https://github.com/bitwiseshiftleft/sjcl">SJCL</a> which is only used to generate cryptographically secure random numbers. It is published under the MIT licence. <a href="https://github.com/thinktt/enigmaX">This is it's github page.</a> The online Enigma simulators by <a href="http://enigma.louisedade.co.uk/enigma.html">Louise Dade</a>, <a href="http://startpad.googlecode.com/hg/labs/js/enigma/enigma-sim.html">Mike Koss</a> and <a href="http://enigmaco.de/enigma/enigma.swf">Frank Spiess</a> were all very helpful while coding this. Also thanks to great community at stackoverflow who helped me solve my CSS and JavaScript problems.

