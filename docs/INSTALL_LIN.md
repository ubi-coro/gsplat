## <img src="https://seeklogo.com/images/T/tux-logo-AA06C623EC-seeklogo.com.png" height="20" /> Installation

> [!NOTE]
>
> Please install [Pytorch](https://pytorch.org/get-started/locally/) first.

1. The easiest way is to install from PyPI. In this way it will build the CUDA code **on the first run** (JIT).

    ```bash
    pip install gsplat
    ```

2. Alternatively you can install gsplat from source. In this way it will build the CUDA code during installation.

    ```bash
    pip install git+https://github.com/nerfstudio-project/gsplat.git
    ```

3. We also provide [pre-compiled wheels](https://docs.gsplat.studio/whl) for both linux and windows on certain python-torch-CUDA combinations (please check first which versions are supported). Note this way you would have to manually install [gsplat's dependencies](https://github.com/nerfstudio-project/gsplat/blob/6022cf45a19ee307803aaf1f19d407befad2a033/setup.py#L115). For example, to install gsplat for pytorch 2.0 and cuda 11.8 you can run

    ```bash
    pip install ninja numpy jaxtyping rich
    pip install gsplat --index-url https://docs.gsplat.studio/whl/pt20cu118
    ```