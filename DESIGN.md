# Snr design

Snr is split into several components:

 - libsnr: the core of snr. both the interface and the generated payloads use it thoroughly. [Component's DESIGN.md](https://github.com/GlobularOne/libsnr/blob/main/DESIGN.md)

 - snr: the text-based interface for snr, a (dare I say, beautiful) shell-like environment with a good list of commands. [Component's DESIGN.md](https://github.com/GlobularOne/snr/blob/main/DESIGN.md)

 - snr_payloads: the default set of payloads, that can be used from within the interface [Component's DESIGN.md](https://github.com/GlobularOne/snr_payloads/blob/main/DESIGN.md)

The release's major controls compatibility. For example, snr pre-release (0.X.X) is not going to work with libsnr version 1 (1.X.X).
