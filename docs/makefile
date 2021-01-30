all: render publish

render:
	Rscript -e 'rmarkdown::render_site()'

publish:	
	RSCRIPT -e 'fs::dir_copy("docs", new_path = "docs", overwrite = T)'