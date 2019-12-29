---
title: {{ cookiecutter.title }}
author: 
{%- for author in cookiecutter.author_full_names_separated_by_commas.split(",") %}
  - {{ author.lstrip() }}
{%- endfor %}
{%- if cookiecutter.double_spacing != "n" or cookiecutter.double_spacing != "n" %}
header-includes:
{%- endif %}
{%- if cookiecutter.double_spacing != "n" %}
  - \usepackage{setspace}
  - \doublespacing
{%- endif %}
{%- if cookiecutter.line_numbers != "n"%}
  - \usepackage[left]{lineno}
  - \linenumbers
{%- endif %}
{%- if cookiecutter.margin_inches != "default" %}
geometry: margin={{cookiecutter.margin_inches}}in
{%- endif %}
{%- if cookiecutter.font_size != "default" %}
fontsize: {{cookiecutter.font_size}}pt
{%- endif %}
{%- if cookiecutter.two_columns != "n" %}
classoption: twocolumn
{%- endif %}
bibliography: bibliography.bib
{%- if cookiecutter.bibliography_style != "Default LaTeX" %}
csl: style.csl
{%- endif %}
{%- if cookiecutter.abstract == "y" %}
{%- if cookiecutter.include_lorem_ipsum != "n" %}
abstract: |
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
  Mattis pellentesque id nibh tortor id aliquet lectus proin nibh. 
  Tellus id interdum velit laoreet id donec. 
  Id velit ut tortor pretium viverra suspendisse potenti. 
  Ipsum nunc aliquet bibendum enim facilisis. 
  Viverra nibh cras pulvinar mattis nunc sed blandit libero volutpat. 
  Id diam maecenas ultricies mi eget mauris pharetra et ultrices. 
  Consequat interdum varius sit amet mattis. 
  Erat velit scelerisque in dictum non consectetur a erat nam. 
  Mi eget mauris pharetra et ultrices neque ornare. 
  In ante metus dictum at.
{%- else %}
abstract: ""
{%- endif -%}
{%- endif %}
---

{%- if cookiecutter.include_standard_paper_headings %}

# Introduction

{% if cookiecutter.include_lorem_ipsum != "n" -%}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua [@Lee2018].
Mattis pellentesque id nibh tortor id aliquet lectus proin nibh.
Tellus id interdum velit laoreet id donec.
Id velit ut tortor pretium viverra suspendisse potenti.
Ipsum nunc aliquet bibendum enim facilisis.
Viverra nibh cras pulvinar mattis nunc sed blandit libero volutpat.
Id diam maecenas ultricies mi eget mauris pharetra et ultrices.
Consequat interdum varius sit amet mattis.
Erat velit scelerisque in dictum non consectetur a erat nam.
Mi eget mauris pharetra et ultrices neque ornare.
In ante metus dictum at.

Mauris vitae ultricies leo integer malesuada nunc vel.
Orci nulla pellentesque dignissim enim sit amet.
Malesuada pellentesque elit eget gravida cum.
A arcu cursus vitae congue.
Donec ultrices tincidunt arcu non sodales neque sodales ut etiam.
Purus faucibus ornare suspendisse sed nisi lacus sed viverra.
Sit amet venenatis urna cursus eget nunc scelerisque viverra mauris.
Bibendum est ultricies integer quis.
Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices.
Turpis massa sed elementum tempus egestas sed sed risus pretium.
Integer eget aliquet nibh praesent tristique magna.
Diam maecenas sed enim ut.
Adipiscing commodo elit at imperdiet dui accumsan sit.
Felis eget nunc lobortis mattis.
Diam quam nulla porttitor massa id.
Volutpat consequat mauris nunc congue.
Nunc sed id semper risus in hendrerit gravida rutrum.
Iaculis eu non diam phasellus.
Auctor augue mauris augue neque gravida.

Mollis nunc sed id semper risus in hendrerit gravida.
Pellentesque pulvinar pellentesque habitant morbi tristique senectus et netus.
Velit egestas dui id ornare arcu odio ut sem nulla.
Nec ullamcorper sit amet risus.
Hendrerit dolor magna eget est lorem.
Quam viverra orci sagittis eu volutpat.
Egestas congue quisque egestas diam in arcu cursus.
Natoque penatibus et magnis dis parturient montes.
Cursus turpis massa tincidunt dui ut ornare lectus sit amet.
Enim neque volutpat ac tincidunt vitae semper.
Varius duis at consectetur lorem.
Urna id volutpat lacus laoreet non curabitur.
Elit scelerisque mauris pellentesque pulvinar pellentesque.
Neque vitae tempus quam pellentesque nec nam aliquam.
Massa eget egestas purus viverra accumsan in.
Aliquam sem et tortor consequat id porta.
Faucibus interdum posuere lorem ipsum.

Aliquet porttitor lacus luctus accumsan tortor posuere ac ut.
Pellentesque sit amet porttitor eget dolor.
Tempus imperdiet nulla malesuada pellentesque elit eget gravida cum.
Habitasse platea dictumst vestibulum rhoncus est pellentesque elit ullamcorper dignissim.
Habitant morbi tristique senectus et.
Elit scelerisque mauris pellentesque pulvinar pellentesque habitant morbi tristique.
Tellus in metus vulputate eu.
Risus quis varius quam quisque id diam.
Eget magna fermentum iaculis eu non.
Curabitur gravida arcu ac tortor dignissim convallis aenean.
Eget velit aliquet sagittis id consectetur.
Gravida neque convallis a cras.
Tincidunt ornare massa eget egestas purus.
Ac turpis egestas integer eget aliquet nibh praesent tristique magna.
Integer malesuada nunc vel risus commodo.

Tristique et egestas quis ipsum suspendisse ultrices gravida.
Faucibus scelerisque eleifend donec pretium.
Elementum curabitur vitae nunc sed velit dignissim sodales ut eu.
Quam pellentesque nec nam aliquam sem.
Dictum sit amet justo donec enim diam vulputate.
Enim ut tellus elementum sagittis vitae.
Tincidunt augue interdum velit euismod.
In eu mi bibendum neque egestas congue.
Ac placerat vestibulum lectus mauris ultrices.
Mauris cursus mattis molestie a.
Velit sed ullamcorper morbi tincidunt ornare massa.
Blandit libero volutpat sed cras ornare arcu.
Vitae ultricies leo integer malesuada nunc vel risus commodo viverra.
Quis auctor elit sed vulputate mi sit amet mauris.
Mus mauris vitae ultricies leo integer malesuada nunc.
Etiam sit amet nisl purus in mollis.»
Feugiat nibh sed pulvinar proin.
Egestas pretium aenean pharetra magna ac placerat vestibulum lectus.
Viverra maecenas accumsan lacus vel facilisis volutpat est velit.
Ac felis donec et odio.
{%- endif %}

# Methods

{% if cookiecutter.include_lorem_ipsum != "n" -%}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Mattis pellentesque id nibh tortor id aliquet lectus proin nibh.
Tellus id interdum velit laoreet id donec.
Id velit ut tortor pretium viverra suspendisse potenti.
Ipsum nunc aliquet bibendum enim facilisis.
Viverra nibh cras pulvinar mattis nunc sed blandit libero volutpat.
Id diam maecenas ultricies mi eget mauris pharetra et ultrices.
Consequat interdum varius sit amet mattis.
Erat velit scelerisque in dictum non consectetur a erat nam.
Mi eget mauris pharetra et ultrices neque ornare.
In ante metus dictum at.

Mauris vitae ultricies leo integer malesuada nunc vel.
Orci nulla pellentesque dignissim enim sit amet.
Malesuada pellentesque elit eget gravida cum.
A arcu cursus vitae congue.
Donec ultrices tincidunt arcu non sodales neque sodales ut etiam.
Purus faucibus ornare suspendisse sed nisi lacus sed viverra.
Sit amet venenatis urna cursus eget nunc scelerisque viverra mauris.
Bibendum est ultricies integer quis.
Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices.
Turpis massa sed elementum tempus egestas sed sed risus pretium.
Integer eget aliquet nibh praesent tristique magna.
Diam maecenas sed enim ut.
Adipiscing commodo elit at imperdiet dui accumsan sit.
Felis eget nunc lobortis mattis.
Diam quam nulla porttitor massa id.
Volutpat consequat mauris nunc congue.
Nunc sed id semper risus in hendrerit gravida rutrum.
Iaculis eu non diam phasellus.
Auctor augue mauris augue neque gravida.

Mollis nunc sed id semper risus in hendrerit gravida.
Pellentesque pulvinar pellentesque habitant morbi tristique senectus et netus.
Velit egestas dui id ornare arcu odio ut sem nulla.
Nec ullamcorper sit amet risus.
Hendrerit dolor magna eget est lorem.
Quam viverra orci sagittis eu volutpat.
Egestas congue quisque egestas diam in arcu cursus.
Natoque penatibus et magnis dis parturient montes.
Cursus turpis massa tincidunt dui ut ornare lectus sit amet.
Enim neque volutpat ac tincidunt vitae semper.
Varius duis at consectetur lorem.
Urna id volutpat lacus laoreet non curabitur.
Elit scelerisque mauris pellentesque pulvinar pellentesque.
Neque vitae tempus quam pellentesque nec nam aliquam.
Massa eget egestas purus viverra accumsan in.
Aliquam sem et tortor consequat id porta.
Faucibus interdum posuere lorem ipsum.

Aliquet porttitor lacus luctus accumsan tortor posuere ac ut.
Pellentesque sit amet porttitor eget dolor.
Tempus imperdiet nulla malesuada pellentesque elit eget gravida cum.
Habitasse platea dictumst vestibulum rhoncus est pellentesque elit ullamcorper dignissim.
Habitant morbi tristique senectus et.
Elit scelerisque mauris pellentesque pulvinar pellentesque habitant morbi tristique.
Tellus in metus vulputate eu.
Risus quis varius quam quisque id diam.
Eget magna fermentum iaculis eu non.
Curabitur gravida arcu ac tortor dignissim convallis aenean.
Eget velit aliquet sagittis id consectetur.
Gravida neque convallis a cras.
Tincidunt ornare massa eget egestas purus.
Ac turpis egestas integer eget aliquet nibh praesent tristique magna.
Integer malesuada nunc vel risus commodo.

Tristique et egestas quis ipsum suspendisse ultrices gravida.
Faucibus scelerisque eleifend donec pretium.
Elementum curabitur vitae nunc sed velit dignissim sodales ut eu.
Quam pellentesque nec nam aliquam sem.
Dictum sit amet justo donec enim diam vulputate.
Enim ut tellus elementum sagittis vitae.
Tincidunt augue interdum velit euismod.
In eu mi bibendum neque egestas congue.
Ac placerat vestibulum lectus mauris ultrices.
Mauris cursus mattis molestie a.
Velit sed ullamcorper morbi tincidunt ornare massa.
Blandit libero volutpat sed cras ornare arcu.
Vitae ultricies leo integer malesuada nunc vel risus commodo viverra.
Quis auctor elit sed vulputate mi sit amet mauris.
Mus mauris vitae ultricies leo integer malesuada nunc.
Etiam sit amet nisl purus in mollis.
Feugiat nibh sed pulvinar proin.
Egestas pretium aenean pharetra magna ac placerat vestibulum lectus.
Viverra maecenas accumsan lacus vel facilisis volutpat est velit.
Ac felis donec et odio.
{%- endif %}

# Results

{% if cookiecutter.include_lorem_ipsum != "n" -%}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Mattis pellentesque id nibh tortor id aliquet lectus proin nibh.
Tellus id interdum velit laoreet id donec.
Id velit ut tortor pretium viverra suspendisse potenti.
Ipsum nunc aliquet bibendum enim facilisis.
Viverra nibh cras pulvinar mattis nunc sed blandit libero volutpat.
Id diam maecenas ultricies mi eget mauris pharetra et ultrices.
Consequat interdum varius sit amet mattis.
Erat velit scelerisque in dictum non consectetur a erat nam.
Mi eget mauris pharetra et ultrices neque ornare.
In ante metus dictum at.

Mauris vitae ultricies leo integer malesuada nunc vel.
Orci nulla pellentesque dignissim enim sit amet.
Malesuada pellentesque elit eget gravida cum.
A arcu cursus vitae congue.
Donec ultrices tincidunt arcu non sodales neque sodales ut etiam.
Purus faucibus ornare suspendisse sed nisi lacus sed viverra.
Sit amet venenatis urna cursus eget nunc scelerisque viverra mauris.
Bibendum est ultricies integer quis.
Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices.
Turpis massa sed elementum tempus egestas sed sed risus pretium.
Integer eget aliquet nibh praesent tristique magna.
Diam maecenas sed enim ut.
Adipiscing commodo elit at imperdiet dui accumsan sit.
Felis eget nunc lobortis mattis.
Diam quam nulla porttitor massa id.
Volutpat consequat mauris nunc congue.
Nunc sed id semper risus in hendrerit gravida rutrum.
Iaculis eu non diam phasellus.
Auctor augue mauris augue neque gravida.

Mollis nunc sed id semper risus in hendrerit gravida.
Pellentesque pulvinar pellentesque habitant morbi tristique senectus et netus.
Velit egestas dui id ornare arcu odio ut sem nulla.
Nec ullamcorper sit amet risus.
Hendrerit dolor magna eget est lorem.
Quam viverra orci sagittis eu volutpat.
Egestas congue quisque egestas diam in arcu cursus.
Natoque penatibus et magnis dis parturient montes.
Cursus turpis massa tincidunt dui ut ornare lectus sit amet.
Enim neque volutpat ac tincidunt vitae semper.
Varius duis at consectetur lorem.
Urna id volutpat lacus laoreet non curabitur.
Elit scelerisque mauris pellentesque pulvinar pellentesque.
Neque vitae tempus quam pellentesque nec nam aliquam.
Massa eget egestas purus viverra accumsan in.
Aliquam sem et tortor consequat id porta.
Faucibus interdum posuere lorem ipsum.

Aliquet porttitor lacus luctus accumsan tortor posuere ac ut.
Pellentesque sit amet porttitor eget dolor.
Tempus imperdiet nulla malesuada pellentesque elit eget gravida cum.
Habitasse platea dictumst vestibulum rhoncus est pellentesque elit ullamcorper dignissim.
Habitant morbi tristique senectus et.
Elit scelerisque mauris pellentesque pulvinar pellentesque habitant morbi tristique.
Tellus in metus vulputate eu.
Risus quis varius quam quisque id diam.
Eget magna fermentum iaculis eu non.
Curabitur gravida arcu ac tortor dignissim convallis aenean.
Eget velit aliquet sagittis id consectetur.
Gravida neque convallis a cras.
Tincidunt ornare massa eget egestas purus.
Ac turpis egestas integer eget aliquet nibh praesent tristique magna.
Integer malesuada nunc vel risus commodo.

Tristique et egestas quis ipsum suspendisse ultrices gravida.
Faucibus scelerisque eleifend donec pretium.
Elementum curabitur vitae nunc sed velit dignissim sodales ut eu.
Quam pellentesque nec nam aliquam sem.
Dictum sit amet justo donec enim diam vulputate.
Enim ut tellus elementum sagittis vitae.
Tincidunt augue interdum velit euismod.
In eu mi bibendum neque egestas congue.
Ac placerat vestibulum lectus mauris ultrices.
Mauris cursus mattis molestie a.
Velit sed ullamcorper morbi tincidunt ornare massa.
Blandit libero volutpat sed cras ornare arcu.
Vitae ultricies leo integer malesuada nunc vel risus commodo viverra.
Quis auctor elit sed vulputate mi sit amet mauris.
Mus mauris vitae ultricies leo integer malesuada nunc.
Etiam sit amet nisl purus in mollis.
Feugiat nibh sed pulvinar proin.
Egestas pretium aenean pharetra magna ac placerat vestibulum lectus.
Viverra maecenas accumsan lacus vel facilisis volutpat est velit.
Ac felis donec et odio.
{%- endif %}

# Discussion

{% if cookiecutter.include_lorem_ipsum != "n" -%}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Mattis pellentesque id nibh tortor id aliquet lectus proin nibh.
Tellus id interdum velit laoreet id donec.
Id velit ut tortor pretium viverra suspendisse potenti.
Ipsum nunc aliquet bibendum enim facilisis.
Viverra nibh cras pulvinar mattis nunc sed blandit libero volutpat.
Id diam maecenas ultricies mi eget mauris pharetra et ultrices.
Consequat interdum varius sit amet mattis.
Erat velit scelerisque in dictum non consectetur a erat nam.
Mi eget mauris pharetra et ultrices neque ornare.
In ante metus dictum at.

Mauris vitae ultricies leo integer malesuada nunc vel.
Orci nulla pellentesque dignissim enim sit amet.
Malesuada pellentesque elit eget gravida cum.
A arcu cursus vitae congue.
Donec ultrices tincidunt arcu non sodales neque sodales ut etiam.
Purus faucibus ornare suspendisse sed nisi lacus sed viverra.
Sit amet venenatis urna cursus eget nunc scelerisque viverra mauris.
Bibendum est ultricies integer quis.
Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices.
Turpis massa sed elementum tempus egestas sed sed risus pretium.
Integer eget aliquet nibh praesent tristique magna.
Diam maecenas sed enim ut.
Adipiscing commodo elit at imperdiet dui accumsan sit.
Felis eget nunc lobortis mattis.
Diam quam nulla porttitor massa id.
Volutpat consequat mauris nunc congue.
Nunc sed id semper risus in hendrerit gravida rutrum.
Iaculis eu non diam phasellus.
Auctor augue mauris augue neque gravida.

Mollis nunc sed id semper risus in hendrerit gravida.
Pellentesque pulvinar pellentesque habitant morbi tristique senectus et netus.
Velit egestas dui id ornare arcu odio ut sem nulla.
Nec ullamcorper sit amet risus.
Hendrerit dolor magna eget est lorem.
Quam viverra orci sagittis eu volutpat.
Egestas congue quisque egestas diam in arcu cursus.
Natoque penatibus et magnis dis parturient montes.
Cursus turpis massa tincidunt dui ut ornare lectus sit amet.
Enim neque volutpat ac tincidunt vitae semper.
Varius duis at consectetur lorem.
Urna id volutpat lacus laoreet non curabitur.
Elit scelerisque mauris pellentesque pulvinar pellentesque.
Neque vitae tempus quam pellentesque nec nam aliquam.
Massa eget egestas purus viverra accumsan in.
Aliquam sem et tortor consequat id porta.
Faucibus interdum posuere lorem ipsum.

Aliquet porttitor lacus luctus accumsan tortor posuere ac ut.
Pellentesque sit amet porttitor eget dolor.
Tempus imperdiet nulla malesuada pellentesque elit eget gravida cum.
Habitasse platea dictumst vestibulum rhoncus est pellentesque elit ullamcorper dignissim.
Habitant morbi tristique senectus et.
Elit scelerisque mauris pellentesque pulvinar pellentesque habitant morbi tristique.
Tellus in metus vulputate eu.
Risus quis varius quam quisque id diam.
Eget magna fermentum iaculis eu non.
Curabitur gravida arcu ac tortor dignissim convallis aenean.
Eget velit aliquet sagittis id consectetur.
Gravida neque convallis a cras.
Tincidunt ornare massa eget egestas purus.
Ac turpis egestas integer eget aliquet nibh praesent tristique magna.
Integer malesuada nunc vel risus commodo.

Tristique et egestas quis ipsum suspendisse ultrices gravida.
Faucibus scelerisque eleifend donec pretium.
Elementum curabitur vitae nunc sed velit dignissim sodales ut eu.
Quam pellentesque nec nam aliquam sem.
Dictum sit amet justo donec enim diam vulputate.
Enim ut tellus elementum sagittis vitae.
Tincidunt augue interdum velit euismod.
In eu mi bibendum neque egestas congue.
Ac placerat vestibulum lectus mauris ultrices.
Mauris cursus mattis molestie a.
Velit sed ullamcorper morbi tincidunt ornare massa.
Blandit libero volutpat sed cras ornare arcu.
Vitae ultricies leo integer malesuada nunc vel risus commodo viverra.
Quis auctor elit sed vulputate mi sit amet mauris.
Mus mauris vitae ultricies leo integer malesuada nunc.
Etiam sit amet nisl purus in mollis.
Feugiat nibh sed pulvinar proin.
Egestas pretium aenean pharetra magna ac placerat vestibulum lectus.
Viverra maecenas accumsan lacus vel facilisis volutpat est velit.
Ac felis donec et odio.
{%- endif %}
{%- endif %}

# References
