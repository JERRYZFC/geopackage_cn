![OGC Logo](http://portal.opengeospatial.org/files/?artifact_id=11976&format=gif "OGC Logo")

GeoPackage 规范
==========
本规范描述了一个开放的、基于标准的、独立于平台的、轻便的、自描述的、传输地理空间信息的压缩格式。
它是基于SQLite的约定集合，目的是在通用平台上[base](spec/1_base.md)存储具有互操作性的[Features](spec/2_features.md) 和/或 [Tiles](spec/3_tiles.md) 数据。
核心文件还额外指定了可选的[Metadata](spec/5_metadata.md) 和[Schema](spec/4_schema.md)信息来构建更丰富的应用。
[Extension Mechanism](spec/7_extensions-mechanism.md)包括一些可选的[extensions](spec/8_extensions.md)，主要是为实现者提供一种方式，这种方式可以使他们的GeoPackages增加额外的功能。

该规范的HTML版本可在地址 http://opengis.github.io/geopackage/ 中得到。

中文翻译说明 Chinese Translation Introduction
-----
本GitHub资料库的目的是对OGC GeoPackage资料库(https://github.com/opengis/geopackage) 做完整的中文翻译，便于中文传播。
除README.md的本小结（中文翻译说明）外，都基于GeoPackage规范原文忠实翻译，未对GeoPackage原文的意思做任何增、删、变动。
GeoPackage规范的版权和知识产权都属于OGC。

This GitHub repository is build to translate the Original OGC GeoPackage repository(https://github.com/opengis/geopackage) to Chinese, so that the GeoPackage Specification can be more widespread.
The translation will not do any changes to the original geopackage repository on implication except this ‘Chinese Translation Introduction’ chapter.

该规范的英文HTML版本（原版）可在地址 http://opengis.github.io/geopackage/ 中得到。
该规范的中文HTML版本可在地址 http://supermap.github.io/geopackage_cn/ 中得到。

HTML version of the spec is available at http://opengis.github.io/geopackage/
HTML version of the Chinese spec is available at http://supermap.github.io/geopackage_cn/

关于
-----

这个GitHub资料库最初摘录自Microsoft Word版本，它的候选GeoPackage标准版本0.8（[version 0.8](https://portal.opengeospatial.org/files/?artifact_id=54838) ）于2013年8月6日发布，是为了公开征求建议（[public comment](http://www.opengeospatial.org/standards/requests/105) ）。
有了这个资料库，OGC可以邀请用户直接参与协作和评论，这使得这个候选标准得以发展和提高。

随着规范的发展，repo不断跟踪最新版本的规范。我们欢迎为修该规范而发的Pull请求，在1.0(2014第一季度)版本定稿后，新的功能也将予以考虑。
该规范被转换成了一种github支持的[asciidoc](http://www.methods.co.nz/asciidoc/) 纯文本格式，github中该规范以章节为单位拆分成几个纯文本文件，这样拆分在某些方面使文档显示更加规范，如自动章节编号。

**Editor: Paul Daisey**

阅读文档
--------------------
主要规范可以在地址 http://opengis.github.io/geopackage/中阅读。
规范的asciidoc源文件在spec/文件目录下。


贡献
------------
贡献者应该了解；任何贡献，一旦被OGC成员接受，就会纳入正式的OGC GeoPackage 标准文件中，所有的版权和知识产权都属于OGC。

该GeoPackage标准工作组（GeoPackage Standards Working Group ，SWG）是OGC中负责本规范管理工作的组，而该组正在努力做尽可能多的公开的GeoPackage工作。

Geopackage SWG目前有以下的邮件列表：
   - geopackage@lists.opengeospatial.org -- [sign up here](https://lists.opengeospatial.org/mailman/listinfo/geopackage)
      - 公开列表
      - 公开归档
      - 没有知识产权的项目应该在这里讨论
   - geopackage.swg@lists.opengeospatial.org -- [sign up here](https://lists.opengeospatial.org/mailman/listinfo/geopackage.swg)
      - 私有列表
      - 访问控制的归档
      - 需要OGC成员和观察员协议来保护知识产权(intellectual property rights, IPR)

编辑和评论
----------------------
该GeoPackage SWG通过GitHub接受公众的意见和建议去修改规范。这是OGC第一次使用该机制向公众征求意见和审查。
在对该规范提交修改性建议时，请先fork本仓库，然后提交修改本文档的pull请求。
请针对每一个逻辑修改，都做一次pull请求，以及确保在PR上有一条评论，评论要包含你支持这种改变的原因或理由。

如需更详细的指南，或者如果你是github新手，请查看 [Process page](process.md)了解更多编辑时的附加信息。

示例实现
----------------------

[Luciad](http://www.luciad.com/)已经把它们的实现[libgpkg](https://bitbucket.org/luciad/libgpkg)开源。[libgpkg](https://bitbucket.org/luciad/libgpkg)完整地支持要素，瓦片，空间索引等。

GDAL(http://www.gdal.org/) 支持geopackage的实现位于 [github repository](https://github.com/pramsey/gdal/tree/gpkg) ，正在开发中。

GeoPackage 示例数据
----------------------
[Sigma Bravo](http://www.sigmabravo.com.au/services/it.aspx) 创建了[Haiti OSM tiles and points](https://portal.opengeospatial.org/files/?artifact_id=52605) geopackage 示例数据。

