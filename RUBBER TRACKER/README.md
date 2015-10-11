Team Name:

RUBBER TRACKER

Project Description:

TLDR: project unsuccessful, but created a Ruby downloading utility

This project's goal is a script for downloading a set of samples from the
Converse Rubber Tracks Sample Library into a 64-pad
Ableton Live Drum Rack in the style of the [Infinite Drum Rack](http://producerdj.com/product/infinite-drum-rack-live-9/) from [ill.Gates](http://producerdj.com/). This layout for finger drumming standardizes the locations of various parts (kicks, snares, etc.) and allows for easy cycling of samples so you can dial in a tight kit from a large range of samples.

Since Ableton Live 9.2 exposes all 64 pads on the Push controller in a drum rack, it's possible to access a large number of samples in a routine.

Progress:

I started out building a ruby utility for parsing API messages and downloading files to build drum racks. This project is here:

http://github.com/hybernaut/rubber_tracks

Unfortunately I was working on the assumption that all samples would be organized in packages, but many of the samples I examined did not contain package references.

I also learned that the Ableton ADG file format is gzip xml, quite readable, and incredibly comprehensive. It should be easy to generate a file describing a drum rack which Ableton Live would accept, with links to the downloaded samples properly laid out on the grid.

Unfortunately the ADG format uses a block of binary data in the <FileRef> element which I could not decipher, so I was unable to complete this part of the project.

URL:

http://github.com/hybernaut/rubber_tracks

Individual Name / Email:

Brian Del Vecchio <bdv@hybernaut.com>
