**Evented JavaScript for the browser**

This script adds the EventEmitter class to your browser. It has the same API and functionality as the NodeJS implementation.

So you can listen for and emit events from what ever objects you choose.

## API

### addListener(eventName, listener)

Assigns a listener to the specified event

 * param {String} eventName Name of the event to assign the listener to
 * param {Function} listener Function to be executed when the specified event is emitted
 * returns {Object} The current instance of EventEmitter to allow chaining

### on(eventName, listener)

Assigns a listener to the specified event (alias for addListener)

 * param {String} eventName Name of the event to assign the listener to
 * param {Function} listener Function to be executed when the specified event is emitted
 * returns {Object} The current instance of EventEmitter to allow chaining

### once(eventName, listener)

Assigns a listener to the specified event removes its self after the first run

 * param {String} eventName Name of the event to assign the listener to
 * param {Function} listener Function to be executed when the specified event is emitted
 * returns {Object} The current instance of EventEmitter to allow chaining

### emit(eventName)

Emits the specified event running all listeners associated with it

 * param {String} eventName Name of the event to execute the listeners of
 * param {Mixed} arguments You can pass as many arguments as you want after the event name. These will be passed to the listeners
 * returns {Object} The current instance of EventEmitter to allow chaining

### listeners(eventName)

Returns an array of listeners for the specified event name

 * param {String} eventName Name of the event to get the listeners for
 * returns {Array} An array of listeners for the specified event

## removeListener(eventName, listener)

Removes the specified listener

 * param {String} eventName Name of the event to remove the listener from
 * param {Function} listener Listener function to be removed
 * returns {Object} The current instance of EventEmitter to allow chaining

## removeAllListeners(eventName)

Removes all listeners from the specified event

 * param {String} eventName Name of the event to remove the listeners from
 * returns {Object} The current instance of EventEmitter to allow chaining

## Tests

EventEmitter is tested and working in the following browsers.

 * Chrome
 * Firefox
 * Safari
 * Opera
 * IE 5 - 9

If you test it in something a little more obscure, please let me know how it turned out.

To test, simply run `test.html` in the test folder.

## Author

[Oliver Caldwell](http://olivercaldwell.co.uk/).

## Licences

### MIT
Copyright (C) 2011 Oliver Caldwell

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

### GPL
Copyright (C) 2011 Oliver Caldwell

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.