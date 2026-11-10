# Nakliyat Platformu Taşınma Teklifleri Veri Seti

**Moving Quotes Dataset (Türkiye)**

Sürüm / Version: **2026-10** (1 Kasım 2025 – 31 Ekim 2026 / 1 November 2025 – 31 October 2026). Lisans / License: CC BY 4.0.

## Türkçe

Türkiye'de Nakliyat Platformu'nda açılan ev taşıma taleplerine platforma kayıtlı nakliyecilerin verdiği tekliflerden hesaplanan aylık toplu istatistikler: şehir içi ve şehirler arası, ev tipine ve ile göre teklif aralığı (%25–%75) ve ortanca teklif, en çok talep gelen güzergâhlar, il merkezleri arası karayolu mesafesi bandına göre şehirler arası teklifler, kat ve asansör durumuna göre şehir içi 2+1 ve 3+1 teklifler, çıkış ilçesine göre şehir içi teklifler (tüm ev tipleri birlikte), teklif alma oranı, talep başına teklif sayısı ve ilk teklif süresi. Rakamlar verilen tekliflerdir; anlaşılan veya ödenen fiyat değildir. Her hücre en az 20 talep, 20 farklı müşteri ve 10 nakliyeciye dayanır; kişisel veri içermez. Sürüm 2026-10: 1 Kasım 2025–31 Ekim 2026; talep verisinin %89'u Haziran–Eylül 2026'ya aittir.

## English

Aggregate statistics, released monthly, computed from the quotes that movers registered on Nakliyat Platformu submitted in response to home-moving requests opened on the platform in Türkiye: within-city and intercity quote ranges (25th–75th percentile) and median quote by home type and province, most-requested routes, intercity quotes by road-distance band between province centres, within-city quotes for 2+1 and 3+1 homes (rooms + living room) by floor and lift status, within-city quotes by origin district (all home types combined), share of requests receiving at least one quote, quotes per request and time to first quote. Figures are quotes given, not agreed or paid prices. Each cell is based on at least 20 requests, 20 distinct customers and 10 movers; the dataset contains no personal data. Version 2026-10 covers 1 November 2025 – 31 October 2026; 89% of the request data is from June–September 2026.

## Sürümler / Versions

Bu depo her ay yeni sürümle güncellenir; resmî ve en güncel sürüm https://www.evdennakliyateve.com/veri/ adresindedir. Kalıcı arşiv: Zenodo, tüm sürümler için DOI 10.5281/zenodo.24111330, bu sürüm için DOI 10.5281/zenodo.24111331.

This repository is updated monthly; the official and latest version is at https://www.evdennakliyateve.com/veri/. Permanent archive: Zenodo, DOI 10.5281/zenodo.24111330 for all versions, DOI 10.5281/zenodo.24111331 for this version.

## Dosyalar / Files

Dosyalar: altı tablo iki biçimde — virgüllü UTF-8 .csv ve Excel için -excel.csv (noktalı virgül, UTF-8 BOM); platform-sayilari.csv (nakliyeci hesabı sayıları; hesap sayısıdır, firma sayısı değil) yalnız virgüllü .csv. tasinma-teklifleri.json yedi tablonun tamamını ve sözlüğü içerir; veri-sozlugu.csv kolon tanımlarını Türkçe ve İngilizce verir. kat-etkisi.csv'deki gruplar yan yana verilir; bina tipi de farklı olduğundan aradaki fark katın ya da asansörün etkisi olarak okunmamalıdır.

Files: six tables in two formats — comma-separated UTF-8 .csv and -excel.csv for Excel (semicolon, UTF-8 BOM); platform-sayilari.csv (mover account counts; accounts, not companies) as comma-separated .csv only. tasinma-teklifleri.json contains all seven tables and the data dictionary; veri-sozlugu.csv gives column definitions in Turkish and English. Groups in kat-etkisi.csv are shown side by side; because building types also differ, differences between them should not be read as the effect of floor or lift.


## Kullanım / Usage

```python
import pandas as pd

url = "https://raw.githubusercontent.com/nakliyatplatformu/tasinma-teklifleri/main/nakliyat-teklif-araliklari.csv"
df = pd.read_csv(url)
```

## Bağlantılar / Links

- Resmî sayfa / Official page: https://www.evdennakliyateve.com/veri/
- Yöntem / Methodology: https://www.evdennakliyateve.com/veri/yontem/
- Sürüm arşivi / Version archive: https://www.evdennakliyateve.com/veri/arsiv/
- Zenodo: https://doi.org/10.5281/zenodo.24111330
- Wikidata: https://www.wikidata.org/wiki/Q142103212
- Hugging Face: https://huggingface.co/datasets/nakliyat-platformu/tasinma-teklifleri

## Kaynak gösterimi / Citation

Kaynak: Nakliyat Platformu, Taşınma Teklifleri Veri Seti, Ekim 2026 sürümü (1 Kasım 2025–31 Ekim 2026), CC BY 4.0 — https://www.evdennakliyateve.com/veri/ — doi:10.5281/zenodo.24111331

Source: Nakliyat Platformu, Moving Quotes Dataset (Türkiye), version 2026-10 (1 November 2025 – 31 October 2026), CC BY 4.0 — https://www.evdennakliyateve.com/veri/ — doi:10.5281/zenodo.24111331

```bibtex
@dataset{nakliyat_platformu_tasinma_teklifleri_2026_10,
  author    = {{Nakliyat Platformu}},
  title     = {Nakliyat Platformu Taşınma Teklifleri Veri Seti},
  version   = {2026-10},
  year      = {2026},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.24111331},
  url       = {https://www.evdennakliyateve.com/veri/}
}
```
