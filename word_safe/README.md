# Word-Safe

Prevents words from being longer than a certain length

## Usage

### `{exp:word_safe}`

#### Example Usage

```
{exp:word_safe length="25" option="breakup"}

    {comment}

{/exp:word_safe}
```

#### Parameters

##### `length`

Maximum character length for a word (default is 25).
- `option` - What to do with words that exceed the maximum length.
 * `option="breakup"` - Breaks up word with spaces. No chunk will ever exceed the maximum length.
 * `option="remove"` - Removes the word
 * `option="shorten"` (default) - Removes any characters after the maximum length has been reached

##### `safe_pre`

(y/n)  If set to 'y' (default), any content in a <pre> tag are exempt from the maximum word length rule. If set to 'n', then the contents of a <pre> tag are treated like any other content.

##### `safe_urls`

(y/n) - If set to 'y' (default), the content in <a> and <img> tags are ignored and thus the URLs are safe from the maximum word length. If set to 'n', then the contents of the <a> and <img> tags will be treated likes words.

## Change Log

### 2.0

- Updated plugin to be 3.0 compatible

### 1.3

- Updated plugin to be 2.0 compatible

### 1.2

- Fixed bug where entities were being broken up, just like a boy band.

### 1.1

- Fixed bug where the breakup setting the letter at the break was duplicated.
