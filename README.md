# Signal Filter

Signal Filter is a lightweight, open-source tool for extracting meaningful signals from text. It identifies key action items, decisions, and risks — helping you cut through noise.

## Usage

```python
from signal_filter.analyzer import SignalAnalyzerPro

analyzer = SignalAnalyzerPro()
result = analyzer.analyze(
    "We decided to reject the delay. The team agreed upon the approved deadline."
)

for item in result.items:
    print(f"[{item.score}] {item.content}")
