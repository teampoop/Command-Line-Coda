# Command-Line Coda

Command-Line Coda is a script for [Panic](http://panic.com)'s Coda. It allows you to open files in Coda from the command line.

## Usage

	coda [a list of files or directories you want to open]

	coda myfile.txt                   # coda creates files if they don't exist
	coda somedir                      # if you specify a directory, coda will open all files in that directory
	coda file1.txt file2.txt somedir3 # you can open multiple files

## Install

	gem install coda

## Setting Coda's path

By default, we assume that Coda lives at `/Applications/Coda.app`. To override this path, set the `CODAPATH` variable:
The following examples are for use with Coda 2.

	CODAPATH="/Applications/Coda 2.app" coda test.txt

Put the following line in your .bash_profile so you don't have to set it every time.

	export CODAPATH="/Applications/Coda 2.app"
  
Written by [Aditya Bhargava](http://adit.io). No warranty is implied, use at your own risk.
