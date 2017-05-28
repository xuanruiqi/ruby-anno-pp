# Ruby Annotations Preprocessor for Markdown

Irritated by the difficulty to write ruby annotations, I decided to just do it myself.

Since Markdown doesn't have built-in support for ruby annotations, all ruby annotations are 
transformed into raw HTML. Therefore, you need to use a raw HTML-supporting compiler for 
Markdown (e.g., Kramdown).

## Requirements
Python 3

## Syntax
`[Base Text]|(Base Text)|（Base Text）|【Base Text】{Annotation}|｛Annotation｝`  
Base text can only contain Chinese characters, Hiragana and Katakana, or the 
preprocesssor will fail. Annotation can contain anything, but of course except for 
the curly braces "}" and "｝".

## Usage
`mdruby [input_file]`. This tool prints to standard output; it is recommended to 
use standard output redirection.

## License
MIT License. See "LICENSE" file.