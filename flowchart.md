```mermaid

flowchart TD
    A(Input Forest Point Cloud) --> B(Semantic Segmentation: PointNet++)
    B --> C(Terrain)
    B --> D(Vegetation)
    B --> E("Coarse Woody Debris (CWD)")
    B --> F(Stems)
    F --> G(Stem Skeletonization)
    G --> H(Individual Tree Segmentation)
    H --> I(Extract Measurements: Height, DBH, Volume)