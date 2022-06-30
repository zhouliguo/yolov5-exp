# Changes

## train.py 

line 490 disable AutoAnchor parser.add_argument('--noautoanchor', action='store_true', default=True, help='disable AutoAnchor')

## utils/loss.py 

line 120 add the image/feature ratio self.ifratio = torch.tensor([8,16,32],device=device)

line 140 and 141 change the calculation of the length and width in training

line 179 rewrite the build_targets function

## models/yolo.py

line 68 and 69 change the calculation of the length and width in val/test

line 124 comment out this line

