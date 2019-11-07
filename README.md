# mqueue
A simple queue for your shell scripts.

## Install
Clone the repo and put the `mpush`, `mpeek`, and `mpop` files somewhere in your PATH.

## Usage
### Push
```
echo 'Hello' | mpush my_queue
echo 'World' | mpush my_queue
```

### Peek
```
mpeek my_queue   # Prints 'Hello'
```

### Pop
```
mpop my_queue    # Prints 'Hello'
mpop my_queue    # Prints 'World'
```

## Warning
The items are stored in a directory with the same name that you specify as the queue name. So, be careful to choose a unique name that does not conflict with your existing directories.

If you run `mpop` on a directory that happens to have a file named like `0000000001`, it will be deleted. You have been warned!

## Version History
+ **1.0**
	+ Initial release.

## Author
**Soheil Rashidi**

+ http://soheilrashidi.com
+ http://twitter.com/soheilpro
+ http://github.com/soheilpro

## Copyright and License
Copyright 2019 Soheil Rashidi.

Licensed under the The MIT License (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

http://www.opensource.org/licenses/mit-license.php

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
