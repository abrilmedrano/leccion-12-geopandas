# GeoPandas

El repositorio correspondiente a esta lección está disponible en [https://github.com/tpb708-programacionsig-2020/leccion-12-geopandas/](https://github.com/tpb708-programacionsig-2020/leccion-12-geopandas/). Se recomienda bifurcarlo a su cuenta en GitHub.

## Recursos
- Sitio web de GeoPandas: [GeoPandas](https://geopandas.org/)

## Notebooks
- [GeoPandas](https://github.com/tpb708-programacionsig-2020/leccion-12-geopandas/blob/master/geopandas.ipynb)
- [GeoPandas - gráficos y mapas](https://github.com/tpb708-programacionsig-2020/leccion-12-geopandas/blob/main/geopandas-graficos-mapas.ipynb)

## Creación de un ambiente Conda y clonación del repositorio
Ejecute estos comandos desde la línea de comandos de Anaconda, en el directorio en el que desea almacenar el repositorio clonado.
```shell
# Actualización de Conda
conda update -n base -c defaults conda

# Creación del ambiente
conda create -n leccion-12a

# Activación del ambiente
conda activate leccion-12a

# Instalación de módulos
# GeoPandas, Jupyter, Git
conda config --env --add channels conda-forge
conda config --env --set channel_priority strict
conda install python=3 geopandas matplotlib descartes jupyter git folium

# Clonación del repositorio (debe sustituir la palabra "usuario" por su nombre de usuario en GitHub)
git clone https://github.com/usuario/leccion-12-geopandas.git
cd leccion-12-geopandas

# Prueba de carga de los módulos en el interpretador de Python (los import no deben producir errores)
python
>>> import pandas
>>> import geopandas
>>> import matplotlib
>>> import descartes
>>> quit()

# Ejecución del Jupyter Notebook
jupyter notebook

# Actualización del repositorio y de los archivos GeoJSON generados
git add .
git commit -m "Actualizar notebook"
git push

# Desactivación del ambiente Conda
conda deactivate
```
