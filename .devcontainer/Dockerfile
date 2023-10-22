FROM jupyter/minimal-notebook

# Copy environment.yml (if found) to a temp location so we update the environment.
COPY codespaces.yml* /tmp/conda-tmp/

RUN mamba env update --name base --file /tmp/conda-tmp/codespaces.yml

# [Optional] Uncomment to install a different version of Python than the default
# RUN conda install -y python=3.6 \
#     && pip install --no-cache-dir pipx \
#     && pipx reinstall-all

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>
