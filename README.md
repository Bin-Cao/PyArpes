# PyArpes
Data Post-Processing Package for ARPES Data

Tutorial : ./tutorial.ipynb

```
Signature:
show.Igor.dispersion(
    self,
    file_loc,
    Columns_range=None,
    E_photon=25,
    work_function=4.28,
    E_Bind=0,
    alpha=1,
    beta=-8.11399,
    Rows=834,
    R_Start=-2.2675,
    R_Delta=0.003,
    R_Units='Kinetic Energy [eV]',
    Columns=489,
    C_Start=-17.6403,
    C_Delta=0.0682412,
    C_Units='Y-Scale [deg]',
    cmap='coolwarm',
    fontsize=16,
)
Docstring:
Visualize the ARPES dispersion data as a colormap.

Reference:
    Zhang H, Pincelli T, Jozwiak C, et al. Angle-resolved photoemission spectroscopy[J]. Nature Reviews Methods Primers, 2022, 2(1): 54.

Parameters:
    file_loc (str): Path to the data file containing the ARPES data.
    Columns_range (list, optional): Range of column values to display (e.g., [-14, 15]).
    E_photon (float): Energy of incident photon in eV (default is 25 eV).
    work_function (float): Work function of the instrument in eV (default is 4.28 eV).
    E_Bind (float): Binding energy of electrons in eV (default is 0 eV).
    alpha (float): Angle alpha in degrees (default is 1°).
    beta (float): Angle beta in degrees (default is -8.11399°).
    Rows (int): Number of rows (N) in the data (default is 834).
    R_Start (float): Starting value for rows (energy in eV) (default is -2.2675 eV).
    R_Delta (float): Step size for rows (energy step in eV) (default is 0.003 eV).
    R_Units (str): Units for rows (default is 'Kinetic Energy [eV]').
    Columns (int): Number of columns (M) in the data (default is 489).
    C_Start (float): Starting value for columns (Y-scale angle in degrees) (default is -17.6403°).
    C_Delta (float): Step size for columns (angle step in degrees) (default is 0.0682412°).
    C_Units (str): Units for columns (default is 'Y-Scale [deg]').
    cmap (str): Colormap style for the plot (default is 'coolwarm').
    fontsize (int): Font size for labels, title, and ticks (default is 14).

Returns:
    None: Displays the plot and saves it to files.

E.g.,
    PyArpes.Igor().dispersion(file_loc = './data.txt')
```