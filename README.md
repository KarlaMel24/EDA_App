# EDA_App
Repository of EDA Application in streamlit



*Notes and recomendations:*

I had many issues with the packages, so I'm sharing the changes I made in case someone is experimenting the same issues.
- It's important to remember that **ydata-profiling** is the new name of the package.
- **ydata-profiling** needs the numba dependency 'generated_jit', but that dependency is being deprecated in numba=0.59, so I needed the version numba=0.58.1.
- **numba=0.58.1** doesn't work on Python>12, so, it's necessary to use a python versions that's 3.8.x <= or < 3.12, in my case, I use python=11.8. I made an environment with that version in conda.
- It's necessary to uninstall and install **pyarrow** so it works again. It's also necessary to import it in the code.



Until now, the app runs locally, but not in streamlit-io, that's why I'm not adding a link. If that changes, I will upload this file.
