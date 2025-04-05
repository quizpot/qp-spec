<h1 align="center">
  Specification
</h1>


Here you will find everything about the `.qp` file.

## Format

The file has a JSON format which stores everything about the quiz in a single file.

# File Contents

## Version

`file.version` is the version of the file format in an integer format. This is checked by the editor and the game logic to make sure the file is compatible with underlying logic.

## Title

`file.title` the title of the quiz in a string format with variable length.

## Description

`file.description` is the description of the quiz in a string format with variable length.

## Thumbnail

`file.thumbnail` is the base64 encoded thumbnail image of the quiz.

## Background

`file.background` can be a base64 encoded background image of the quiz or a hexadecimal color code used as a background of the quiz.

## Language

`file.language` is the language of the quiz in ISO 639 format used for metadata purposes.

## Questions

`file.questions` is an array of questions.

### Question

An object that represents a question in the quiz. Contains the following properties:

`question.questionType` is the type of the question is an enum of the available question types.
`question.timeLimit` is the time limit in seconds for the question.
`question.points` is the points mode for the question.
