Learning about quantization. Coding samples from HuggingFace quantization courses.

Finished Courses:
1. _HF Quantization Fundamentals_: [https://www.deeplearning.ai/short-courses/quantization-fundamentals-with-hugging-face/]
- Basic quantization techniques in PyTorch
- PyTorch types (int8, float, bfloat16...) --> review these
- using "quanto"

2. _HF Quantization in Depth_: [https://www.deeplearning.ai/short-courses/quantization-in-depth/]
- Linear quantization
- Asymmetric Linear: r = s(q - z); q = int(round(r/s + z))
    - trade-off: more complex, memory to save zero point: but better use of quantization range
- Symmetric Linear: q = int(round(r/s)); s = rmax/qmax (no zero point)
- Per-channel, per-group options
- Building 8-bit quantizer (8W16A)
- Replace PyTorch linear layers with quantized layer
- Quantizing open-source models
- Weights packing algorithm

(These Medium articles are basically the HF tutorial with some extra explanation)
- [https://medium.com/@sayedebad.777/the-power-of-quantization-in-ml-a-pytorch-tutorial-part-1-8d0c1bf8b679]
- [https://medium.com/@sayedebad.777/the-power-of-quantization-in-ml-a-pytorch-tutorial-part-2-3557ffb1249f]
- [https://medium.com/@sayedebad.777/the-power-of-quantization-in-ml-a-pytorch-tutorial-part-3-9b7dba23e067]
- [https://medium.com/@sayedebad.777/the-power-of-quantization-in-ml-a-pytorch-tutorial-part-4-ae521e8a00ae]
- [https://medium.com/@sayedebad.777/the-power-of-quantization-in-ml-a-pytorch-tutorial-part-5-204883da375f]

- Intel neural compressor: [https://github.com/intel/neural-compressor/blob/master/docs/source/quantization.md]
- HF Chart: [https://huggingface.co/docs/transformers/v4.45.2/quantization/overview]
- PyTorch Basics (Review): [https://pytorch.org/blog/quantization-in-practice/]

Next to go through:

AMD Docs:
1. AMD Quark: [https://quar.docs.amd.com]
2. AMD ROCm: [https://rocm.docs.amd.com/en/latest]

Other Docs:
1. PyTorch Quantization: [https://pytorch.org/docs/stable/quantization.html]
2. intel/neural-compressor: [https://github.com/intel/neural-compressor/tree/master]
3. huggingface/optimum-quanto: [https://github.com/huggingface/optimum-quanto]
4. NVIDIA/TensorRT-Model-Optimizer: [https://github.com/NVIDIA/TensorRT-Model-Optimizer/]
5. vllm-project/vllm: [https://github.com/vllm-project/vllm]

Research blogs in similar areas:
- HF blog
- PyTorch blog
- PyTorch dev forum
- NVIDIA blog
- AI research from Intel
- AI research from Qualcomm
