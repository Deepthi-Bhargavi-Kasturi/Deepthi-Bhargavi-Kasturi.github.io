
<h1>Transformers</h1>

<p>We can select the model to be used in a pipeline for a specific task.</p>

from transformers import pipeline
generator = pipeline("text-generation", model="HuggingFaceTB/SmolLM2-360M")

generator(
  "Cats are cute"
  max_new_tokens=25,
  num_return_sequences=2
)


model can be selected for a specific task and also languages can be selected from model <a href="https://huggingface.co/models?pipeline_tag=text-generation&language=ja,fr,en&sort=trending">hub</a>

