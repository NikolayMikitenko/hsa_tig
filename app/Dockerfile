# Starting from base miniconda image
FROM continuumio/miniconda3
# Setting working directory in destination
WORKDIR /app
# This is the complete set of libraries required
RUN conda install panel
#
RUN ls
# Copy the relevant folder into the container
COPY . .
# Run panel serve to start the app
#CMD panel serve --address="0.0.0.0" --port=$PORT main.py --allow-websocket-origin=worldbank-climate-dashboard.herokuapp.com
CMD panel serve --allow-websocket-origin=localhost:20015 --port 20015 app.py