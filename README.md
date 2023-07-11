# Dataset of "small" lattice polytopes

Resulting dataset from the paper [Enumeration of Lattice Polytopes by Their Volume](https://arxiv.org/abs/1811.03357).

edit: it is recommended to download the dataset from [Zenodo](https://zenodo.org/record/7388010#.Y4kbP3bMJOQ) as it is compressed and requires no extra postprocessing due to github size limit

## Cite as

Balletti, G. Enumeration of Lattice Polytopes by Their Volume. Discrete Comput Geom 65, 1087–1122 (2021). [[doi](https://doi.org/10.1007/s00454-020-00187-y), [arXiv](https://arxiv.org/abs/1811.03357)].

## Content

It contains the following complete datasets of lattice polytopes, see the paper for additional details.

 - 2-simplices up to volume 1000
 - 3-simplices up to volume 1000
 - 4-simplices up to volume 24
 - 5-simplices up to volume 20
 - 6-simplices up to volume 16
 - 2-polytopes up to volume 50
 - 3-polytopes up to volume 36
 - 4-polytopes up to volume 24
 - 5-polytopes up to volume 20
 - 6-polytopes up to volume 16
 - Smooth 2-polytopes up to volume 50
 - Smooth 3-polytopes up to volume 36
 - Smooth 4-polytopes up to volume 24
 - Smooth 5-polytopes up to volume 20
 - Smooth 6-polytopes up to volume 16

## Be careful

* Each polytope is saved as the sequence of its vertices, as in the following example.
    
      [[0,0],[1,0],[0,1],[1,1]]
    
* Simplices and polytopes are listed by their volume, e.g. the file ``4-polytopes/v12.txt`` contains all the 4-polytopes having normalized volume equal to 12 (one representative for each equivalence class).
* Each file ends with an empty line.
* In order to keep each file smaller than 50Mb, the files ``v34.txt``, ``v35.txt`` and ``v36.txt`` in ``data/3-polytopes/`` are respectively split in two or three files, e.g ``v34a.txt`` and ``v34b.txt``. Once downloaded they can be joined using cat.

        cat v34a.txt v34b.txt > v34.txt
