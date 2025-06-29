## Required Libraries

```txt
tensorflow
keras
numpy
matplotlib

#### 🧾 Add `pattern_sense.py` Sample in README.md

```markdown
## Main Script

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Flatten, Dense

model = Sequential([
    Conv2D(32, (3, 3), activation='relu', input_shape=(64, 64, 3)),
    MaxPooling2D(2, 2),
    Flatten(),
    Dense(128, activation='relu'),
    Dense(4, activation='softmax')
])
  
