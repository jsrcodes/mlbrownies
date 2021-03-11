

```python
tokenizer = keras.preprocessing.text.Tokenizer(
    filters='',
    oov_token='<oov>'
)
tokenizer.fit_on_texts(text)
tokenized_tensor = tokenizer.text_to_sequences(text)

# Apply padding so that all sequences are of same length.
#The length of the largest string is considered for padding
tokenized_tensor = keras.preprocessing.sequence.pad_sequences(
    tensor, padding='post'
)

```
