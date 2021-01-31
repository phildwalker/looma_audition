all: render commit

render:
	Rscript -e 'rmarkdown::render_site()'

publish:	
	RSCRIPT -e 'fs::dir_copy("docs", new_path = "docs", overwrite = T)'
	
commit:
	git add .; git commit -m "update via make, orange if hover"; git push origin main;