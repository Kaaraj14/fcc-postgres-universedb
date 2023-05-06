--
-- PostgreSQL database dump
--

-- Dumped from database version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
-- Dumped by pg_dump version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    galaxy_id integer NOT NULL,
    name character varying(30) NOT NULL,
    life boolean DEFAULT false,
    for_idx integer,
    size_rate integer NOT NULL
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.galaxy_galaxy_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.galaxy_galaxy_id_seq OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.galaxy_galaxy_id_seq OWNED BY public.galaxy.galaxy_id;


--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    moon_id integer NOT NULL,
    name character varying(30) NOT NULL,
    description text,
    for_idx integer,
    color character varying(20)
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.moon_moon_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.moon_moon_id_seq OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.moon_moon_id_seq OWNED BY public.moon.moon_id;


--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    planet_id integer NOT NULL,
    name character varying(30) NOT NULL,
    num_moons integer,
    sun_num integer,
    numeric_data numeric,
    habitable boolean,
    for_idx integer
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.planet_planet_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.planet_planet_id_seq OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.planet_planet_id_seq OWNED BY public.planet.planet_id;


--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    star_id integer NOT NULL,
    name character varying(30) NOT NULL,
    description text,
    for_idx integer,
    type character varying(20)
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.star_star_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.star_star_id_seq OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.star_star_id_seq OWNED BY public.star.star_id;


--
-- Name: tab5; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.tab5 (
    tab5_id integer NOT NULL,
    collective_id integer NOT NULL,
    name character varying(30)
);


ALTER TABLE public.tab5 OWNER TO freecodecamp;

--
-- Name: tab5_tab5_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.tab5_tab5_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.tab5_tab5_id_seq OWNER TO freecodecamp;

--
-- Name: tab5_tab5_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.tab5_tab5_id_seq OWNED BY public.tab5.tab5_id;


--
-- Name: galaxy galaxy_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy ALTER COLUMN galaxy_id SET DEFAULT nextval('public.galaxy_galaxy_id_seq'::regclass);


--
-- Name: moon moon_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon ALTER COLUMN moon_id SET DEFAULT nextval('public.moon_moon_id_seq'::regclass);


--
-- Name: planet planet_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet ALTER COLUMN planet_id SET DEFAULT nextval('public.planet_planet_id_seq'::regclass);


--
-- Name: star star_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star ALTER COLUMN star_id SET DEFAULT nextval('public.star_star_id_seq'::regclass);


--
-- Name: tab5 tab5_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.tab5 ALTER COLUMN tab5_id SET DEFAULT nextval('public.tab5_tab5_id_seq'::regclass);


--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES (2, 'milky way', true, 1, 1);
INSERT INTO public.galaxy VALUES (3, 'andromeda', false, 2, 2);
INSERT INTO public.galaxy VALUES (4, 'eso_270-17', false, 3, 4);
INSERT INTO public.galaxy VALUES (5, 'cosmos_red', false, 4, 3);
INSERT INTO public.galaxy VALUES (6, 's_megallanic', false, 5, 2);
INSERT INTO public.galaxy VALUES (7, 'l_megallanic', false, 6, 3);
INSERT INTO public.galaxy VALUES (8, 'mil way', true, 12, 1);
INSERT INTO public.galaxy VALUES (9, 'ndromeda', false, 11, 2);
INSERT INTO public.galaxy VALUES (10, '\eso_270-17', false, 10, 4);
INSERT INTO public.galaxy VALUES (11, 'osmos_red', false, 9, 3);
INSERT INTO public.galaxy VALUES (12, '_megallanic', false, 8, 2);
INSERT INTO public.galaxy VALUES (13, '_megallanic', false, 7, 3);
INSERT INTO public.galaxy VALUES (14, 'ahsdg', false, 19, 4);
INSERT INTO public.galaxy VALUES (15, 'hgndk', false, 20, 6);
INSERT INTO public.galaxy VALUES (16, 'mil ay', true, 18, 1);
INSERT INTO public.galaxy VALUES (17, 'ndrmeda', false, 17, 2);
INSERT INTO public.galaxy VALUES (18, '\so_270-17', false, 16, 4);
INSERT INTO public.galaxy VALUES (19, 'osmos_red', false, 15, 3);
INSERT INTO public.galaxy VALUES (20, '_megalla\nic', false, 14, 2);
INSERT INTO public.galaxy VALUES (21, '_megallan\ic', false, 13, 3);


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES (1, '1', NULL, 1, NULL);
INSERT INTO public.moon VALUES (2, '2', NULL, 2, NULL);
INSERT INTO public.moon VALUES (3, '3', NULL, 3, NULL);
INSERT INTO public.moon VALUES (4, '4', NULL, 4, NULL);
INSERT INTO public.moon VALUES (5, '5', NULL, 5, NULL);
INSERT INTO public.moon VALUES (6, '6', NULL, 6, NULL);
INSERT INTO public.moon VALUES (7, '7', NULL, 7, NULL);
INSERT INTO public.moon VALUES (8, '8', NULL, 8, NULL);
INSERT INTO public.moon VALUES (9, '9', NULL, 9, NULL);
INSERT INTO public.moon VALUES (10, '10', NULL, 10, NULL);
INSERT INTO public.moon VALUES (11, '11', NULL, 11, NULL);
INSERT INTO public.moon VALUES (12, '12', NULL, 12, NULL);
INSERT INTO public.moon VALUES (13, '13', NULL, 13, NULL);
INSERT INTO public.moon VALUES (14, '14', NULL, 14, NULL);
INSERT INTO public.moon VALUES (15, '15', NULL, 15, NULL);
INSERT INTO public.moon VALUES (16, '16', NULL, 16, NULL);
INSERT INTO public.moon VALUES (17, '17', NULL, 17, NULL);
INSERT INTO public.moon VALUES (18, '18', NULL, 18, NULL);
INSERT INTO public.moon VALUES (19, '19', NULL, 19, NULL);
INSERT INTO public.moon VALUES (20, '20', NULL, 20, NULL);


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES (13, 'earth', NULL, NULL, NULL, NULL, 1);
INSERT INTO public.planet VALUES (14, 'mercury', NULL, NULL, NULL, NULL, 2);
INSERT INTO public.planet VALUES (15, 'venus', NULL, NULL, NULL, NULL, 3);
INSERT INTO public.planet VALUES (16, 'mars', NULL, NULL, NULL, NULL, 4);
INSERT INTO public.planet VALUES (17, 'saturn', NULL, NULL, NULL, NULL, 5);
INSERT INTO public.planet VALUES (18, 'jupiter', NULL, NULL, NULL, NULL, 6);
INSERT INTO public.planet VALUES (19, 'uranus', NULL, NULL, NULL, NULL, 7);
INSERT INTO public.planet VALUES (20, 'neptune', NULL, NULL, NULL, NULL, 8);
INSERT INTO public.planet VALUES (21, 'pl9', NULL, NULL, NULL, NULL, 9);
INSERT INTO public.planet VALUES (22, 'pl10', NULL, NULL, NULL, NULL, 10);
INSERT INTO public.planet VALUES (23, 'pl11', NULL, NULL, NULL, NULL, 11);
INSERT INTO public.planet VALUES (24, 'pl12', NULL, NULL, NULL, NULL, 12);
INSERT INTO public.planet VALUES (33, 'eath', NULL, NULL, NULL, NULL, 20);
INSERT INTO public.planet VALUES (34, 'mrcury', NULL, NULL, NULL, NULL, 19);
INSERT INTO public.planet VALUES (35, 'v\enus', NULL, NULL, NULL, NULL, 18);
INSERT INTO public.planet VALUES (36, 'm\ars', NULL, NULL, NULL, NULL, 17);
INSERT INTO public.planet VALUES (37, 'aturn', NULL, NULL, NULL, NULL, 16);
INSERT INTO public.planet VALUES (38, 'jupitr', NULL, NULL, NULL, NULL, 15);
INSERT INTO public.planet VALUES (39, 'ranus', NULL, NULL, NULL, NULL, 14);
INSERT INTO public.planet VALUES (40, 'neptun', NULL, NULL, NULL, NULL, 13);


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES (1, 'sun', NULL, 1, NULL);
INSERT INTO public.star VALUES (2, 'sirius', NULL, 2, NULL);
INSERT INTO public.star VALUES (3, 'vega', NULL, 3, NULL);
INSERT INTO public.star VALUES (4, 'altair', NULL, 4, NULL);
INSERT INTO public.star VALUES (5, 'aries', NULL, 5, NULL);
INSERT INTO public.star VALUES (6, 'rigel', NULL, 6, NULL);
INSERT INTO public.star VALUES (13, 's3n', NULL, 7, NULL);
INSERT INTO public.star VALUES (14, 'siius', NULL, 8, NULL);
INSERT INTO public.star VALUES (15, 'vea', NULL, 9, NULL);
INSERT INTO public.star VALUES (16, 'alt1r', NULL, 10, NULL);
INSERT INTO public.star VALUES (17, 'aris', NULL, 11, NULL);
INSERT INTO public.star VALUES (18, 'rigl', NULL, 12, NULL);
INSERT INTO public.star VALUES (27, 'un', NULL, 20, NULL);
INSERT INTO public.star VALUES (28, 'sirs', NULL, 19, NULL);
INSERT INTO public.star VALUES (29, 'ega', NULL, 18, NULL);
INSERT INTO public.star VALUES (30, 'altar', NULL, 17, NULL);
INSERT INTO public.star VALUES (31, 'aris', NULL, 16, NULL);
INSERT INTO public.star VALUES (32, 'igel', NULL, 15, NULL);
INSERT INTO public.star VALUES (33, 'fhf', NULL, 13, NULL);
INSERT INTO public.star VALUES (34, 'hdks', NULL, 14, NULL);


--
-- Data for Name: tab5; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.tab5 VALUES (1, 1, 'value1');
INSERT INTO public.tab5 VALUES (2, 2, 'value2');
INSERT INTO public.tab5 VALUES (3, 3, 'value');


--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.galaxy_galaxy_id_seq', 21, true);


--
-- Name: moon_moon_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.moon_moon_id_seq', 20, true);


--
-- Name: planet_planet_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.planet_planet_id_seq', 40, true);


--
-- Name: star_star_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.star_star_id_seq', 34, true);


--
-- Name: tab5_tab5_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.tab5_tab5_id_seq', 3, true);


--
-- Name: galaxy galaxy_for_idx_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_for_idx_key UNIQUE (for_idx);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: moon moon_for_idx_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_for_idx_key UNIQUE (for_idx);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: planet planet_for_idx_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_for_idx_key UNIQUE (for_idx);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_for_idx_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_for_idx_key UNIQUE (for_idx);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: tab5 tab5_collective_id_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.tab5
    ADD CONSTRAINT tab5_collective_id_key UNIQUE (collective_id);


--
-- Name: tab5 tab5_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.tab5
    ADD CONSTRAINT tab5_pkey PRIMARY KEY (tab5_id);


--
-- Name: moon moon_for_idx_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_for_idx_fkey FOREIGN KEY (for_idx) REFERENCES public.planet(for_idx);


--
-- Name: planet planet_for_idx_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_for_idx_fkey FOREIGN KEY (for_idx) REFERENCES public.star(for_idx);


--
-- Name: star star_for_idx_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_for_idx_fkey FOREIGN KEY (for_idx) REFERENCES public.galaxy(for_idx);


--
-- PostgreSQL database dump complete
--

