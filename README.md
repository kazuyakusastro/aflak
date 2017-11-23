# Environment

Support Python3.

# Setup

    virtualenv -p python3 venv
    . ./venv/bin/activate

# Open a FITS file

    python aflak.py my-fits-file.fits

The provided FITS file is required to have an extension with the 'FLUX' name.

After some fiddling you should be able to get a window like below:

![Screen capture of the running GUI application](images/2017-11-13-screenshot.jpg?raw=true)


# To see a fits file header

    fold -w 80 foo.fits | less

# TODO

- Distribute through PyPI
- Include CI / code checking tools
- Show arbitrary sums over spectral data (currently only show one frame)
- Benchmark / Test with several fits files
- Include GUI way of loading new images
- Set waveform's X-axis to appropriate units
- Improve ROI drawing