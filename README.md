h2. ����ɻ���

�Ѷ} Dataset\ �ؿ����� ReachOut.zip ���Y�ɡC
���t 1894 ���ɮסC�C���ɮר��@�աA�H�s�� 138717 ���ҡA������� 138717.txt �ɮפ��t�p�U��T�G

```
red	followupWorse

Author:
6315	MemphisBelle
red	followupWorse

LastEditAuthor:
6315	MemphisBelle
Star contributor

Subject:
Re: So what happened.....

Body:
The TV launch was a few weeks ago and it was awesome. One of the rare times in my life I was actually happy and feeling worthwhile....
```

* �Ĥ@�檺 red �N��o�g�峹���ӭn�Q������ red�C
* Author: �N��o�媺�@�� ID
* LastEditAuthor: �N��W���ק諸�@�� ID
* Subject: ��᪺��r�ԭz���o�媺�D��
* Body: ��᪺��r�ԭz���o�媺���e�C

h2. Weka ARFF �ɿ�X

���g�@�{���ಣ�� Weka �� ARFF �ɡA�æۦ�w�q�P��X�p�U�� ARFF ��Ʈ榡�G

```
@relation YOUR RELATION NAME
@attribute Label {green, �K}
@attribute token1 numeric
@attribute token2 numeric
@attribute token3 numeric
�K
@data
{0 green, 1 1, 2 1, �K}
{0 red, 5 1, 9 1, �K}
�K
```

�U���O��ڪ��d�ҡG

```
% Input
% Re : TwittRO It 's not fair @Sophie-RO
%
@relation �d��

@attribute Label {green, xxxx}
@attribute Re numeric
@attribute : numeric
@attribute "TwittRO" numeric
@attribute "It" numeric
@attribute "'s" numeric
@attribute not numeric
@attribute fair numeric
@attribute @Sophie-RO numeric

@data
{0 green, 1 1, 2 1, �K}
...
```

h2. �ϥ� Weka �i�����

�Q�� Weka �� Explorer �f�t�ϥ� Decision Tree, SMO, SimpleLogistic �t��k�i�� 10 fold Cross-validation �Ӵ��էA�]���ҫ������T�v�C