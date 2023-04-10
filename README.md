# Alfred Workflow - Read UTI data

![Read UTI Workflow icon](ReadUTIicon.jpeg)

## Introduction

This workflow was written to help find all of the [Universal Type Identifiers](https://developer.apple.com/documentation/uniformtypeidentifiers) associated with a file type on the Mac. You can read the [details of the problem](https://www.alfredforum.com/topic/20024-file-filter-wont-see-markdown-files-if-the-file-types-is-set/#comment-103460) in this thread on the Alfred forum. 

The Workflow uses a Keyword input and takes the extension (example .svg) for a file type. It then uses the duti command line application to find all of the UTIs associated with that file type and pastes them into the clipboard. 

## Requirements

In order for this Workflow to run you need to have the [duti](http://duti.org) command line application installed on your Mac. The easiest way to do this is to use [Homebrew](https://brew.sh).

`brew install duti` 

## Usage

Bring up the Alfred window and then enter the keyword for the Workflow. The default is `read uti`. 

![read UTI](readUTI.jpg)

Then enter the file extension that you want to get UTI data for.

![readUTI2](readUTI2.jpg)

The Workflow will run and then copy the data it finds into the clipboard. 

## Updates

### version 1.1

Added error checking to make sure that the extension had a . character and that the commands returned text and weren't empty. 


