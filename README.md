# Mac-Torch-GPU-VAE
 Use GPU Acceleration for M1 Macbook.

## Environment Requirement

PyTorch >= 1.12.0

ipykernel (Required)

## Highlighted Calls

```python
# Judge whether GPU is avaiable
if torch.backends.mps.is_available()
	device = torch.device("mps")
else
	device = torch.device("cpu")

# Push model into GPU
model.to(device)
```

