waveinfo
========

waveinfo is a pure-ruby gem to get the information from the headers of Wave (.wav) files.

Installing
----------

You may get the latest stable version from Rubyforge. Source gems are also available.

    $ gem install waveinfo


Synopsis
--------

    require 'rubygems'
    require 'waveinfo'
    
    wave = WaveInfo.new('example.wav')
    puts "Channels: #{wave.channels}"
    puts "Sample Rate: #{wave.sample_rate} Hz"
    puts "Duration: #{wave.duration} secs"


TODO
----

* Add support for the extensible format which uses GUIDs
* Inplement more validity checks
  - file is shorter than reported chunk size
  - file is longer than reported chunk size
* Implement more chunk types
  - bext - Broadcast Wave Extention
  - mext - MPEG audio extension chunk
  - DISP - Title
  - cart - CartChunk/aes46-2002
  - LIST
* Test against more weird Wave files


Resources
---------

* GitHub Project: http://github.com/njh/ruby-waveinfo
* Documentation: http://rdoc.info/github/njh/ruby-waveinfo/master/frames

Contact
-------

* Author:    Nicholas J Humfrey
* Email:     njh@aelius.com
* Home Page: http://www.aelius.com/njh/
* License:   Distributes under the same terms as Ruby
