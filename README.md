# Spectral rigidity of finite swap configurations on spheres of revolution

![Zenodo DOI for this paper pending](https://img.shields.io/badge/Zenodo_DOI-pending-lightgrey)

**nunavipahe60-star**

[Read the paper (PDF)](paper.pdf) | [LaTeX source](paper.tex)

Fix a smooth sphere of revolution with a symmetric background profile that increases strictly from the equator to the northern pole. Place finitely many prescribed bumps, with separated support intervals, in either their northern positions or their reflections in the equator. Which choices can one recover from the Laplace spectrum? Every uniqueness statement below allows simultaneous reflection of all the choices.

## Main results

1. **Finite configurations with fixed signs near the edges (Section 3).** If each bump has a fixed sign near each end of its support, one can choose a single ray $\kappa=cM$, $M=|m|$, on which every sufficiently large individual angular weight distinguishes all inequivalent placements. The differences of both the shifted resolvent traces and the normalized log determinants have an exact logarithmic decay rate given by the shortest boundary gap in the ray metric.
2. **Ordinary spectrum of three bumps (Section 4).** For three fixed nonnegative bumps, the ordinary Laplace spectrum with multiplicities determines their placement. This includes the sandwich in which the two latitude gaps have equal length. Odd multiplicities recover the zero sector, while summing over angular weights gives the two gaps different contributions to the full regularized determinant.
3. **Finite branch assignments (Section 5).** For a smooth single well with prescribed sublevel width $W$ and absolute midpoint derivative $|a'|$, suppose the possible sign assignments occur on finitely many interior bands separated by positive gaps, as specified in Section 5. The labelled high-weight spectra determine the branch assignment. The midpoint may take different constant values between bands.
4. **Oscillation at the support edges (Section 7).** Real smooth bumps may change sign infinitely often at their edges. On a ray with unique shortest boundary gap of optical length $d$, the normalized log-determinant difference satisfies $\limsup_{M\to\infty}|\Delta F_M|^{1/M}=e^{-2d}$ along integer weights. Thus arbitrarily large weights distinguish each pair of inequivalent placements. This conclusion allows exceptional weights at which the contrast vanishes.

**Recovery from spectral data (Appendix A).** Two coefficients of the same sector determinant recover the sum of the positive inverse slopes and the sum of their reciprocals at every regular height. These determine the unordered pair of slopes, the width $W$, and $|a'|$. Under the finite-band hypotheses of Section 5, the recovered data and the labelled high-weight spectra together determine the profile up to reflection.

## Related paper

The earlier paper establishes the three-bump result for the equivariant spectrum and introduces the latitude and Mercator gap lengths. Its permanent Zenodo archive is [*Swap pairs on spheres of revolution: what the equivariant spectrum sees* (DOI 10.5281/zenodo.24531890)](https://doi.org/10.5281/zenodo.24531890).

## Build and verify

The source uses pdfLaTeX with an inline bibliography. From the repository root, run the following commands with MiKTeX and a writable build directory.

~~~sh
mkdir build
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=build paper.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=build paper.tex
~~~

The second pass resolves the internal references in `build/paper.pdf`. To verify the distributed files, run `sha256sum -c SHA256SUMS.txt` from the repository root.

## Credits and license

nunavipahe60-star coordinated the research and preparation of the manuscript in collaboration with Claude, Gemini, and Codex. The release includes [citation metadata](CITATION.cff) and the [Apache License, Version 2.0](LICENSE).
