# bninja-cheatsheet
Random notes about binary ninja

# How to add new entries to the dropdown menus

```python

def calculate_entropy_plugin(bv, start, length):
	log_alert(f'Entropy: {bv.get_entropy(start, length)[0]}')

PluginCommand.register_for_range("Calculate Entropy", "Calculate entropy of selected region", calculate_entropy_plugin)

```