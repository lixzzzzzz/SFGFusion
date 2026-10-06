# SFGFusion Project Page

Static academic project page for:

**SFGFusion: Surface fitting guided 3D object detection with 4D radar and camera fusion**  
Pattern Recognition, 2026. DOI: 10.1016/j.patcog.2026.113999

## Preview locally

From the project directory:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a GitHub repository, for example `SFGFusion`.
2. Upload the entire contents of this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then click **Save**.
6. After GitHub finishes deploying, the page will be available at:
   `https://YOUR_GITHUB_USERNAME.github.io/SFGFusion/`

## Publish under PIE Lab domain

The DogMo page is maintained in the `BIT-PIE/DogMo` GitHub repository and is exposed at `https://pie-lab.cn/DogMo/`. To publish SFGFusion in the same style/domain, ask the maintainer of the PIE Lab web hosting / GitHub organization to create the corresponding project repository or route (for example `BIT-PIE/SFGFusion`) and deploy this folder using the same mechanism used for DogMo. The desired final route would be:

`https://pie-lab.cn/SFGFusion/`

The exact final step depends on whether PIE Lab uses GitHub Pages, a reverse proxy, or a server-side static-site mapping for project subpaths.

## Images

The page currently references the figures from the public arXiv HTML version. For a fully self-contained deployment, download these files into `static/images/` and replace the image URLs in `index.html`:

- `Radar_LiDAR_Point_Vis.png`
- `Model_architecture_overall.png`
- `Surface_Fitting_Model.png`
- `Surface_fitting_vis.png`
- `TJ4D_distance.png`
- `TJ4D_vis_result.png`
- `VoD_vis_result.png`
- `Ablation_vis.png`

Source base URL:
`https://arxiv.org/html/2510.19215v1/`

## Optional edits

- Replace the disabled `Code · coming soon` button with the final public code repository URL.
- Add author profile links for Huijun Di, Jian Li, and Feng Liu if desired.
- If you want an exact PIE Lab visual match, keep the Bulma CDN and the current section hierarchy; the page is intentionally modeled after the DogMo academic project page.

## Attribution

The visual structure is adapted from the open-source project-page template used by DogMo:
`https://github.com/silverster98/project-page-template`

Template license: CC BY-SA 4.0.
